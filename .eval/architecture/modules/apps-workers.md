# Module: apps/workers [AI]

(part 1 of 3) Executes asynchronous background tasks, scheduled maintenance, and metadata processing for Karakeep. It manages distributed workers for link crawling, metadata/reader view extraction, full-text and asset preprocessing (OCR and PDF parsing), AI inference/embeddings jobs, backups, webhooks, and administrative data maintenance, and can also run as a standalone remote crawler server. (part 2 of 3) Background job queue workers and scheduled tasks for Karakeep that handle webpage crawling, asset and video downloading, RSS feed synchronization, staging bookmark imports, rule evaluation, search indexing, embeddings/tagging orchestration, webhook deliveries, and admin database maintenance. (part 3 of 3) Executes background queue jobs and worker tasks, primarily automated webpage crawling (using Patchright headless browser, metadata probing, monolith archiving, and optional remote crawler HTTP API) and AI inference operations (automatic tagging and summarization of bookmarks).

_This module does not fit in one model call, so it was read in 3 parts and their summaries were combined without a further model call._

## Key files
- `apps/workers/index.ts`: Entry point that initializes telemetry, loads plugins, prepares queues, and orchestrates the lifecycle of all configured background workers, scheduled cron workers, or the remote crawler server.
- `apps/workers/server.ts`: Configures and starts the Hono HTTP server exposing health check (/health), Prometheus metric (/metrics), and optional remote crawler routes.
- `apps/workers/network.ts`: Provides SSRF-safe HTTP fetching, IP address range validation, DNS resolution caching, and socket address pinning.
- `apps/workers/workers/assetPreprocessingWorker.ts`: Processes asset queue tasks including PDF text extraction, screenshot generation, and image OCR via Tesseract or LLM inference.
- `apps/workers/workers/backupWorker.ts`: Handles automated daily/weekly backup scheduling and executes data export packaging into compressed archives.
- `apps/workers/workers/adminMaintenanceWorker.ts`: Executes administrative maintenance tasks like tidying unreferenced assets, quota purges, and migrating large HTML link content.
- `apps/workers/scripts/parseHtmlSubprocess.ts`: Subprocess script executing Metascraper, DOMPurify, Defuddle, and Readability extraction on HTML documents in an isolated environment.
- `apps/workers/workers/crawlerWorker.ts`: Processes link crawl jobs by downloading remote web pages and assets, extracting metadata, and enqueueing downstream search, embedding, video, and AI tagging jobs.
- `apps/workers/workers/embeddingsWorker.ts`: Generates vector embeddings for bookmarks, stores them in the vector index, and enqueues fallback or follow-up AI tagging tasks in the OpenAI queue.
- `apps/workers/workers/searchWorker.ts`: Indexes and deletes bookmark documents in the full-text search client.
- `apps/workers/workers/feedWorker.ts`: Schedules hourly RSS feed checks and consumes feed queue jobs to parse XML items and ingest new link bookmarks.
- `apps/workers/workers/importWorker.ts`: Polls staged import records and processes batch bookmark imports with concurrency controls, fair user scheduling, and backpressure management.
- `apps/workers/workers/ruleEngineWorker.ts`: Evaluates user-configured automation rules on bookmark lifecycle events.
- `apps/workers/workers/videoWorker.ts`: Downloads video files from supported URLs using yt-dlp and attaches them as asset records under user storage quotas.
- `apps/workers/workers/webhookWorker.ts`: Dispatches HTTP webhook notifications with retry logic on bookmark creation, update, or deletion events.
- `apps/workers/workers/adminMaintenance/tasks/purgeBookmarksOverQuota.ts`: Admin maintenance task that iteratively deletes the oldest bookmarks for users exceeding bookmark quota limits.
- `apps/workers/workers/adminMaintenance/tasks/migrateLinkHtmlContent.ts`: Admin maintenance task that offloads large inline HTML contents from link rows into standalone storage assets.
- `apps/workers/workers/adminMaintenance/tasks/tidyAssets.ts`: Admin maintenance task for removing dangling assets not present in the database or syncing asset metadata.
- `apps/workers/workers/crawler/common.ts`: Defines core Crawler interfaces, CrawlContext types, captured asset configurations, and tracing/logging helpers.
- `apps/workers/workers/crawler/localCrawler.ts`: Implements local crawling using Patchright browser automation, metadata preflight probing, monolith archiving, and subprocess HTML parsing.
- `apps/workers/workers/crawler/remoteCrawler.ts`: Client Crawler implementation that forwards crawl requests to a remote crawler HTTP server via multipart streaming.
- `apps/workers/workers/crawler/remoteCrawlerServer.ts`: Hono HTTP server that exposes endpoints (/probe, /page, /asset, /archive) for running the local crawler remotely.
- `apps/workers/workers/crawler/protocol.ts`: Defines multipart request and response schemas, serialization, and stream reading for the remote crawler protocol.
- `apps/workers/workers/inference/inferenceWorker.ts`: Queue runner for inference jobs, dispatching summarization and tagging tasks and updating bookmark status in Drizzle DB.
- `apps/workers/workers/inference/summarize.ts`: Generates AI summaries for bookmark links using user custom prompts and the shared inference client.
- `apps/workers/workers/inference/tagging.ts`: Performs AI-driven automated tagging on bookmarks (text, links, images, and PDFs) using prompts and the inference client.
- `apps/workers/workers/utils/parseSubprocess.ts`: Executes HTML parsing and content extraction in an isolated Node subprocess with memory constraints.
- `apps/workers/workers/utils/readerViewAssessment.ts`: Scores and classifies whether an HTML document and extracted content are suitable for reader view.

## Public interface
- buildServer(extraRoutes?: Record<string, Hono>): { _server: Server, stop: () => Promise<void>, serve: () => Promise<void> }
- validateUrl(urlCandidate: string, runningInProxyContext: boolean): Promise<UrlValidationResult>
- createPinnedLookup(addresses: string[]): LookupFunction
- getBookmarkDomain(url?: string | null): string | undefined
- withWorkerTracing<TData, TResult>(name: string, fn: (job: DequeuedJob<TData>) => Promise<TResult>): (job: DequeuedJob<TData>) => Promise<TResult>
- withWorkerEventLog<TData, TResult>(name: EventLogType, fn: (job: DequeuedJob<TData>) => Promise<TResult>): (job: DequeuedJob<TData>) => Promise<TResult>
- buildImpersonatingTRPCClient(userId: string): Promise<TRPCClient>
- buildImpersonatingAuthedContext(userId: string): Promise<AuthedContext>
- updateAsset(oldAssetId: string | undefined, newAsset: DBAssetType, txn: KarakeepDBTransaction): void
- getBookmarkDetails(bookmarkId: string): Promise<BookmarkDetails>
- raceWith<T>(work: Promise<T>, ...contenders: RaceContender<T>[]): Promise<T>
- withTimeout<T, Ret>(func: (param: T) => Promise<Ret>, timeoutSec: number): (param: T) => Promise<Ret>
- GET /health
- GET /metrics
- CrawlerWorker
- EmbeddingsWorker
- FeedRefreshingWorker
- FeedWorker
- ImportWorker
- RuleEngineWorker
- SearchIndexingWorker
- VideoWorker
- WebhookWorker
- runMigrateLargeLinkHtmlTask
- runPurgeBookmarksOverQuotaTask
- runTidyAssetsTask
- Crawler interface and CrawlContext (apps/workers/workers/crawler/common.ts)
- localCrawler (apps/workers/workers/crawler/localCrawler.ts)
- remoteCrawler (apps/workers/workers/crawler/remoteCrawler.ts)
- buildRemoteCrawlerRoutes (apps/workers/workers/crawler/remoteCrawlerServer.ts)
- OpenAiWorker (apps/workers/workers/inference/inferenceWorker.ts)
- runSummarization (apps/workers/workers/inference/summarize.ts)
- runTagging (apps/workers/workers/inference/tagging.ts)
- runParseSubprocess (apps/workers/workers/utils/parseSubprocess.ts)
- assessReaderView (apps/workers/workers/utils/readerViewAssessment.ts)
- parseFeedItems (apps/workers/workers/utils/feedParser.ts)
- fetchAllBookmarksForUser and fetchBookmarksInBatches (apps/workers/workers/utils/fetchBookmarks.ts)

## Dependencies
- @karakeep/db
- @karakeep/shared
- @karakeep/shared-server
- @karakeep/trpc
- @hono/node-server
- @hono/prometheus
- hono
- prom-client
- node-fetch
- http-proxy-agent
- https-proxy-agent
- ipaddr.js
- lru-cache
- drizzle-orm
- archiver
- node-cron
- @paralleldrive/cuid2
- cheerio
- html-entities
- zod
- metascraper
- metascraper-amazon
- metascraper-author
- metascraper-date
- metascraper-description
- metascraper-image
- metascraper-logo-favicon
- metascraper-publisher
- metascraper-title
- metascraper-url
- metascraper-x
- metascraper-youtube
- @mozilla/readability
- defuddle
- dompurify
- jsdom
- winston
- tesseract.js
- pdf2json
- pdf2pic
- @karakeep/db/schema
- @karakeep/shared/config
- @karakeep/shared/inference
- @karakeep/shared/logger
- @karakeep/shared/queueing
- @karakeep/shared/ratelimiting
- @karakeep/shared/search
- @karakeep/shared/tryCatch
- @karakeep/shared/types/bookmarks
- @karakeep/shared/vectorStore
- @karakeep/trpc/lib/impersonate
- @karakeep/trpc/lib/ruleEngine
- @karakeep/trpc/models/bookmarks
- @karakeep/trpc/models/importSessions.service
- @karakeep/trpc/models/webhooks.service
- @trpc/server
- data-uri-to-buffer
- execa
- patchright
- @remix-run/multipart-parser
- @ghostery/adblocker-playwright
- rss-parser
- async-mutex

## AI touchpoints [AI]
- `apps/workers/workers/assetPreprocessingWorker.ts`
- `apps/workers/workers/crawler/localCrawler.ts`
- `apps/workers/workers/crawlerWorker.ts`
- `apps/workers/workers/inference/summarize.ts`
- `apps/workers/workers/inference/tagging.ts`
- `apps/workers/index.ts`
- `apps/workers/workers/embeddingsWorker.ts`
- `apps/workers/workers/inference/inferenceWorker.ts`

## Where the code disagrees with the stack profile
- `apps/workers/server.ts`: The scan reported framework not recognised and server unknown, but the module uses Hono running on @hono/node-server as an HTTP server.; apps/workers includes an HTTP server implemented with Hono and @hono/node-server when CRAWLER_REMOTE_SERVER_ENABLED is active, rather than having an unknown server type.

## Open questions
- How does the worker process lifecycle initialize all workers (crawler, OpenAIWorker, feed parser) at startup outside of remoteCrawlerServer mode?
- Where is the parseHtmlSubprocess entrypoint script located and how does it interface with Defuddle or other extraction libraries?
