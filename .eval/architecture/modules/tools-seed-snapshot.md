# Module: tools/seed-snapshot

Provides CLI tools to generate and apply deterministic seed data snapshots (bookmarks, notes, assets, tags, lists, and highlights) against local or released Karakeep instances for development and migration testing.

## Key files
- `tools/seed-snapshot/src/apply.ts`: CLI script that finds, stages, and extracts the latest or specified seed data archive into the repository's data directory.
- `tools/seed-snapshot/src/index.ts`: CLI generator script that provisions test users and populates bookmarks, lists, tags, and assets via tRPC against a running Karakeep instance to produce snapshot archives and manifests.

## Public interface
- node tools/seed-snapshot/src/apply.ts [--force] [--snapshot <archive-name>]
- node tools/seed-snapshot/src/index.ts [--release <version>] [--replace]

## Dependencies
- @trpc/client
- superjson
- @karakeep/shared/types/bookmarks
- @karakeep/shared/types/lists
- @karakeep/shared/types/tags
- @karakeep/shared/utils/reading-progress-dom
- @karakeep/trpc/routers/_app

## Open questions
- tools/seed-snapshot/src/index.ts is truncated in the provided source, leaving container lifecycle and tarball bundling implementation details incomplete.
