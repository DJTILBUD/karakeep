# Module: packages/open-api

Generates and validates the OpenAPI 3.0 specification for the Karakeep REST API by combining endpoint registries and Zod schemas across bookmarks, lists, tags, highlights, feeds, assets, backups, user profiles, and administrative jobs.

## Key files
- `packages/open-api/index.ts`: Entry point script that aggregates all route registries, builds the OpenAPI 3.0 documentation via OpenApiGeneratorV3, and writes or validates karakeep-openapi-spec.json.
- `packages/open-api/zod-extend.ts`: Bootstraps and extends Zod with OpenAPI schema generation capabilities using @asteasolutions/zod-to-openapi.
- `packages/open-api/lib/bookmarks.ts`: Defines OpenAPI paths and parameter schemas for bookmark management, search (full-text, semantic, hybrid), and retrieval.
- `packages/open-api/lib/admin.ts`: Defines OpenAPI paths for administrative endpoints such as user updates and triggering asynchronous recrawl, search reindexing, and AI inference jobs.
- `packages/open-api/lib/tags.ts`: Defines OpenAPI paths for managing bookmark tags, querying tag usage statistics, and retrieving tagged bookmarks.
- `packages/open-api/lib/lists.ts`: Defines OpenAPI paths for creating, updating, and querying manual and smart (query-based) bookmark lists.
- `packages/open-api/lib/assets.ts`: Defines OpenAPI paths for uploading binary files, downloading assets, and generating temporary signed download URLs.
- `packages/open-api/lib/backups.ts`: Defines OpenAPI paths for initiating, inspecting, downloading, and deleting account zip backups.
- `packages/open-api/lib/feeds.ts`: Defines OpenAPI paths for configuring and manually triggering RSS feed subscriptions that import bookmarks.
- `packages/open-api/lib/highlights.ts`: Defines OpenAPI paths for managing text highlights and associated notes within bookmarks.
- `packages/open-api/lib/users.ts`: Defines OpenAPI paths for fetching current user profile data and account usage statistics.
- `packages/open-api/lib/types.ts`: Shared OpenAPI schemas for core domain objects including PaginatedBookmarks, Highlights, Lists, and pagination params.
- `packages/open-api/lib/common.ts`: Defines shared security schemes such as Bearer JWT authentication.
- `packages/open-api/lib/errors.ts`: Standard error schemas and common unauthorized HTTP response definitions for API documentation.
- `packages/open-api/lib/pagination.ts`: Re-exports pagination and content query parameter schemas from types.ts.

## Public interface
- CLI execution via packages/open-api/index.ts (default writes karakeep-openapi-spec.json; argument 'check' validates existing spec against generated spec)
- registry exports across packages/open-api/lib/*.ts registering OpenAPI path definitions with OpenAPIRegistry

## Dependencies
- @asteasolutions/zod-to-openapi
- zod
- @karakeep/shared/types/admin
- @karakeep/shared/types/backups
- @karakeep/shared/types/bookmarks
- @karakeep/shared/types/feeds
- @karakeep/shared/types/highlights
- @karakeep/shared/types/lists
- @karakeep/shared/types/tags
- @karakeep/shared/types/users

## AI touchpoints [AI]
- `packages/open-api/lib/admin.ts`
- `packages/open-api/lib/bookmarks.ts`

## Open questions
- _none_
