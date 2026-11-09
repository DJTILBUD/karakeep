# Module: packages/api

Provides the Hono-based HTTP REST and tRPC API server for Karakeep, exposing endpoints for bookmarking, asset management and streaming, feed syndication, full text search, admin tasks, webhooks, metrics, and health checks.

## Key files
- `packages/api/index.ts`: Entry point for the Hono application, configuring tracing, CORS, metrics, rate limits, tRPC adapter, and mounting all API route modules under /v1 and other root paths.
- `packages/api/middlewares/auth.ts`: Authentication and authorization middlewares (unauthed, authed, admin) that bind tRPC caller factories to the Hono context.
- `packages/api/middlewares/apiKeyScopes.ts`: Enforces granular API key scope permissions on protected endpoints.
- `packages/api/middlewares/rateLimit.ts`: Applies rate limiting keyed by user ID or IP address via shared ratelimiting client.
- `packages/api/middlewares/readOnlyMode.ts`: Rejects write and mutation requests when the server is in read-only or demo mode.
- `packages/api/middlewares/trpcAdapter.ts`: Converts tRPC errors into appropriate HTTP exception status codes.
- `packages/api/routes/admin.ts`: Handles admin actions including user management and triggering background recrawl, reindex, and inference jobs.
- `packages/api/routes/assets.ts`: Handles asset uploads, signed URL generation, and content streaming with Range support.
- `packages/api/routes/bookmarks.ts`: Manages bookmarks CRUD, search, URL validation, singlefile precrawled archive imports, and chunked readable content retrieval.
- `packages/api/routes/webhooks.ts`: Receives and validates incoming webhooks from Stripe and RevenueCat.
- `packages/api/utils/upload.ts`: Validates MIME types, enforces upload body limits and user storage quotas, and saves uploaded assets to storage.

## Public interface
- default (Hono app instance exported from packages/api/index.ts)
- GET /health
- GET /version
- ALL /trpc/*
- GET /metrics
- POST /webhooks/stripe
- POST /webhooks/revenuecat
- GET /public/assets/:assetId
- v1 REST routes: /v1/highlights, /v1/bookmarks, /v1/lists, /v1/tags, /v1/users, /v1/assets, /v1/admin, /v1/rss, /v1/backups, /v1/feeds

## Dependencies
- @hono/otel
- @hono/prometheus
- @hono/trpc-server
- @hono/zod-validator
- @karakeep/db
- @karakeep/shared
- @karakeep/shared-server
- @karakeep/trpc
- @trpc/server
- file-type
- hono
- prom-client
- rss
- zod

## AI touchpoints [AI]
- `packages/api/routes/admin.ts`

## Open questions
- _none_
