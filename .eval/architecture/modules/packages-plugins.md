# Module: packages/plugins

Provides pluggable infrastructure backends for the application, implementing shared interfaces for asset storage (local filesystem and AWS S3), background job queueing (SQLite via Liteque and distributed workflows via Restate), rate limiting (in-memory and Redis), full text search (MeiliSearch), and vector storage for similarity and semantic search.

## Key files
- `packages/plugins/assetstore-filesystem/src/index.ts`: Implements local filesystem asset storage with path traversal protection, streaming, range reads, and metadata parsing.
- `packages/plugins/assetstore-s3/src/index.ts`: Implements S3 object storage for assets with range reads, metadata synchronization, and bulk cleanup.
- `packages/plugins/queue-liteque/src/index.ts`: Implements local SQLite-backed job queueing and background task execution via liteque.
- `packages/plugins/queue-restate/src/index.ts`: Implements distributed queueing and background workers powered by Restate SDK, including ingress dispatching and priority scheduling.
- `packages/plugins/queue-restate/src/semaphore.ts`: Restate Virtual Object managing job concurrency, priority queues, group fairness, leases, and idempotency.
- `packages/plugins/ratelimit-memory/src/index.ts`: In-memory rate limiter using sliding windows with probabilistic memory cleanup.
- `packages/plugins/ratelimit-redis/src/index.ts`: Distributed Redis rate limiter using atomic Lua scripts and fail-open resilience.
- `packages/plugins/search-meilisearch/src/index.ts`: MeiliSearch client for indexing and full-text searching bookmark documents.
- `packages/plugins/vectorstore-meilisearch/src/index.ts`: MeiliSearch vector store client providing vector insertion, similarity search, and hybrid vector queries.
- `packages/plugins/lib/batchingDocumentQueue.ts`: Thread-safe batched document addition and deletion queue for MeiliSearch operations.

## Public interface
- FileSystemAssetStoreProvider
- LocalFileSystemAssetStore
- S3AssetStoreProvider
- S3AssetStore
- LitequeQueueProvider
- RestateQueueProvider
- RestateQueueClient
- AdminClient
- RateLimitProvider
- RateLimiter
- RedisRateLimitProvider
- RedisRateLimiter
- MeiliSearchProvider
- MeiliSearchVectorProvider
- BatchingDocumentQueue

## Dependencies
- @aws-sdk/client-s3
- @karakeep/shared/assetdb
- @karakeep/shared/config
- @karakeep/shared/logger
- @karakeep/shared/plugins
- @karakeep/shared/queueing
- @karakeep/shared/ratelimiting
- @karakeep/shared/search
- @karakeep/shared/tryCatch
- @karakeep/shared/vectorStore
- @restatedev/restate-sdk
- @restatedev/restate-sdk-clients
- async-mutex
- liteque
- meilisearch
- redis
- zod

## AI touchpoints [AI]
- `packages/plugins/vectorstore-meilisearch/src/index.ts`

## Open questions
- _none_
