# Module: packages/shared-server [AI]

Provides shared server-side utilities, background queue definitions, asset store management, image optimization, quota verification, plugin loading, and OpenTelemetry-based tracing and structured event logging for backend services.

## Key files
- `packages/shared-server/src/plugins.ts`: Loads and initializes server plugins (asset stores, queues, search/vector stores, rate limiters) via PluginManager
- `packages/shared-server/src/assetdb.ts`: Manages asset CRUD operations, read streams, metadata retrieval, and deletion using the registered AssetStore plugin with quota validation
- `packages/shared-server/src/queues.ts`: Declares deferred job queues and Zod schemas for crawling, AI inference, vector embedding generation, search indexing, and administrative maintenance tasks
- `packages/shared-server/src/services/quotaService.ts`: Enforces bookmark count quotas and storage limits across transactions and DB queries
- `packages/shared-server/src/bannerImages.ts`: Optimizes bookmark preview banner images by resizing and converting them to WebP using sharp
- `packages/shared-server/src/eventLogger.ts`: Implements structured contextual event logging with AsyncLocalStorage, Winston, and optional OpenTelemetry OTLP log exporting
- `packages/shared-server/src/tracing.ts`: Provides OpenTelemetry tracing setup, tracer management, and span execution helpers

## Public interface
- loadAllPlugins()
- saveAsset()
- saveAssetFromFile()
- readAsset()
- createAssetReadStream()
- readAssetMetadata()
- getAssetSize()
- deleteAsset()
- deleteUserAssets()
- silentDeleteAsset()
- getAllAssets()
- newAssetId()
- optimizeBannerImage()
- QuotaService
- StorageQuotaError
- LinkCrawlerQueue
- LowPriorityCrawlerQueue
- OpenAIQueue
- EmbeddingsQueue
- SearchIndexingQueue
- AdminMaintenanceQueue
- buildCrawlIdempotencyKey()
- prepareQueue()
- startQueue()
- initEventLogger()
- shutdownEventLogger()
- withEventLog()
- logEvent()
- addLogFields()
- recordEventLogFailure()
- initTracing()
- shutdownTracing()
- getTracer()
- withSpan()
- withSpanSync()
- extractTraceContext()
- injectTraceContext()

## Dependencies
- @karakeep/db
- @karakeep/db/schema
- @karakeep/plugins/assetstore-filesystem
- @karakeep/plugins/assetstore-s3
- @karakeep/plugins/queue-liteque
- @karakeep/plugins/queue-restate
- @karakeep/plugins/ratelimit-memory
- @karakeep/plugins/ratelimit-redis
- @karakeep/plugins/search-meilisearch
- @karakeep/plugins/vectorstore-meilisearch
- @karakeep/shared/assetdb
- @karakeep/shared/config
- @karakeep/shared/logger
- @karakeep/shared/plugins
- @karakeep/shared/queueing
- @karakeep/shared/storageQuota
- @karakeep/shared/types/rules
- @opentelemetry/api
- @opentelemetry/api-logs
- @opentelemetry/exporter-logs-otlp-http
- @opentelemetry/exporter-trace-otlp-http
- @opentelemetry/resources
- @opentelemetry/sdk-logs
- @opentelemetry/sdk-trace-base
- @opentelemetry/sdk-trace-node
- @opentelemetry/semantic-conventions
- @opentelemetry/winston-transport
- @trpc/server
- drizzle-orm
- sharp
- winston
- zod

## AI touchpoints [AI]
- `packages/shared-server/src/eventLogTypes.ts`
- `packages/shared-server/src/tracingTypes.ts`
- `packages/shared-server/src/queues.ts`

## Open questions
- QuotaService notes TODO items to unify its method APIs (return boolean vs throw exception) and to integrate quota approval tokens directly during bookmark creation once moved into the model.
