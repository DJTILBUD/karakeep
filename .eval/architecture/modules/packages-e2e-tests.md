# Module: packages/e2e_tests

(part 1 of 2) End-to-end and integration testing package for the Karakeep bookmarking application, spinning up Docker containers (web, workers, crawler, Meilisearch, Garage S3, Aimock, Nginx) and validating API endpoints, public sharing, asset storage plugins, RSS feeds, backups, and container privileges. (part 2 of 2) End-to-end (E2E) test suite validating the web frontend UI and background worker processing (crawling, AI inference/tagging, vector embeddings, RSS feeds, imports, and video extraction) using Playwright and Vitest.

_This module does not fit in one model call, so it was read in 2 parts and their summaries were combined without a further model call._

## Key files
- `packages/e2e_tests/vitest.config.ts`: Vitest test runner configuration specifying global setup scripts, environment variables, timeouts, and test inclusion patterns.
- `packages/e2e_tests/setup/startContainers.ts`: Global setup harness that dynamically selects free ports, executes Docker Compose to spin up all required backend services, checks health endpoints, and captures container logs on teardown.
- `packages/e2e_tests/setup/seed.ts`: Global setup test project seeder that registers a default admin user and exchanges credentials for an API key.
- `packages/e2e_tests/tests/api/assets.test.ts`: Tests asset upload, retrieval, signed URLs, permission scopes, bookmark attachment, and lifecycle management.
- `packages/e2e_tests/tests/api/bookmarks.test.ts`: Tests CRUD operations, pagination, content cursor streaming/invalidation, and tag operations on bookmarks.
- `packages/e2e_tests/tests/api/feeds.test.ts`: Tests RSS/Atom feed subscription management, manual triggering of feed fetches, and automatic bookmark ingestion.
- `packages/e2e_tests/tests/api/lists.test.ts`: Tests manual and smart list creation, updates, and bookmark list membership.
- `packages/e2e_tests/tests/api/backups.test.ts`: Tests asynchronous backup generation lifecycle, backup polling, downloading, and ZIP structure verification.
- `packages/e2e_tests/tests/api/public.test.ts`: Tests access to public bookmark lists and token-signed public asset retrieval.
- `packages/e2e_tests/tests/api/rss.test.ts`: Tests generation and token authorization of RSS feed endpoints for manual and smart lists.
- `packages/e2e_tests/tests/api/tags.test.ts`: Tests tag creation, pagination, bookmark tagging, and deletion.
- `packages/e2e_tests/tests/api/users.test.ts`: Tests user profile information and user aggregate bookmark statistics.
- `packages/e2e_tests/tests/assetdb/interface-compliance.test.ts`: Validates interface compliance for asset storage plugins (filesystem and S3), including streaming and byte-range reading.
- `packages/e2e_tests/tests/docker/privileges.test.ts`: Inspects running Docker container processes to ensure Next.js and worker processes run with dropped Linux capabilities and restricted privileges.
- `packages/e2e_tests/utils/browser.ts`: Playwright test runner extensions, browser fixtures, DOM navigation/hydration helpers, and test user session setup.
- `packages/e2e_tests/utils/trpc.ts`: Factory for creating typed tRPC test clients against the Karakeep backend API.
- `packages/e2e_tests/utils/api.ts`: HTTP API utility functions for user registration, authentication headers, API key exchange, and test asset uploads.
- `packages/e2e_tests/utils/general.ts`: Polling helper (waitUntil) for testing asynchronous background jobs and state changes.
- `packages/e2e_tests/tests/web/bookmarks.test.ts`: Browser integration tests for saving links/notes, search discovery, and bookmark status toggles.
- `packages/e2e_tests/tests/workers/inference.test.ts`: E2E integration tests verifying automatic AI tagging and summarization execution via worker jobs.
- `packages/e2e_tests/tests/workers/crawler.test.ts`: E2E tests for web page crawling, screenshot generation, PDF creation, and offline archive storage across local and remote engines.
- `packages/e2e_tests/tests/workers/embeddings.test.ts`: E2E tests verifying vector embeddings creation and Meilisearch vector index synchronization.

## Public interface
- setup({ provide }: TestProject) (in packages/e2e_tests/setup/seed.ts)
- default function ({ provide }: TestProject) (in packages/e2e_tests/setup/startContainers.ts)
- createTestAssetData(overrides?) (in packages/e2e_tests/tests/assetdb/assetdb-utils.ts)
- createTestImageData() (in packages/e2e_tests/tests/assetdb/assetdb-utils.ts)
- createTestPdfData() (in packages/e2e_tests/tests/assetdb/assetdb-utils.ts)
- createTempDirectory() (in packages/e2e_tests/tests/assetdb/assetdb-utils.ts)
- cleanupTempDirectory(tempDir) (in packages/e2e_tests/tests/assetdb/assetdb-utils.ts)
- createLocalFileSystemStore(rootPath) (in packages/e2e_tests/tests/assetdb/assetdb-utils.ts)
- createS3Store(bucketName) (in packages/e2e_tests/tests/assetdb/assetdb-utils.ts)
- createTestBucket(bucketName) (in packages/e2e_tests/tests/assetdb/assetdb-utils.ts)
- cleanupTestBucket(s3Client, bucketName) (in packages/e2e_tests/tests/assetdb/assetdb-utils.ts)
- assertAssetExists(store, userId, assetId) (in packages/e2e_tests/tests/assetdb/assetdb-utils.ts)
- assertAssetNotExists(store, userId, assetId) (in packages/e2e_tests/tests/assetdb/assetdb-utils.ts)
- it (extended Vitest test runner with Playwright Page fixture in packages/e2e_tests/utils/browser.ts)
- goto(page: Page, url: string): Promise<void>
- reload(page: Page): Promise<void>
- signIn(page: Page, email: string, password?: string): Promise<void>
- submitSignInForm(page: Page, email: string, password: string): Promise<void>
- waitForHydration(locator: Locator): Promise<void>
- waitForTaggingToFinish(trpc: ReturnType<typeof getTrpcClient>, bookmarkId: string): Promise<void>
- createWebTestUser(): Promise<{ trpc: ReturnType<typeof getTrpcClient>; email: string }>
- bookmarkCards(page: Page): Locator
- bookmarkEditor(page: Page): Locator
- WORKER_TEST_TIMEOUT: number
- createTestUser(scopes?: ZApiKeyScope[], port?: string): Promise<string>
- signUpUser(input: { name: string; email: string; password: string }, port?: string): Promise<void>
- uploadTestAsset(apiKey: string, port: number, file: File): Promise<{ assetId: string; contentType: string; fileName: string }>
- getAuthHeader(apiKey: string): { 'Content-Type': string; authorization: string }
- getTrpcClient(apiKey?: string, port?: string): ReturnType<typeof createTRPCClient<AppRouter>>
- waitUntil(f: () => Promise<boolean>, description: string, timeoutMs?: number): Promise<void>
- createTestPdfFile(fileName?: string): File

## Dependencies
- @karakeep/sdk
- @karakeep/shared
- @karakeep/plugins/assetstore-filesystem
- @karakeep/plugins/assetstore-s3
- vitest
- vite-tsconfig-paths
- @aws-sdk/client-s3
- adm-zip
- zod
- playwright/test
- @karakeep/trpc
- @trpc/client
- superjson

## AI touchpoints [AI]
- `packages/e2e_tests/setup/startContainers.ts`
- `packages/e2e_tests/tests/workers/inference.test.ts`
- `packages/e2e_tests/tests/workers/embeddings.test.ts`

## Open questions
- _none_
