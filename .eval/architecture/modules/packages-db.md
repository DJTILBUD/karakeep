# Module: packages/db

Manages database connections, schema definitions, OpenTelemetry instrumentation, and migrations using SQLite (better-sqlite3) and Drizzle ORM for the self-hosted bookmarking application.

## Key files
- `packages/db/index.ts`: Public entry point exporting the database instance, transaction types, error types, and table schemas
- `packages/db/drizzle.ts`: Initializes and exports the Drizzle ORM database instance and in-memory test database helper
- `packages/db/schema.ts`: Defines SQLite table schemas and relations (users, accounts, sessions, verificationTokens, apiKeys, bookmarks, etc.)
- `packages/db/sqlite.ts`: Configures and opens the better-sqlite3 database connection with pragmas, WAL mode, cache limits, and periodic query optimization
- `packages/db/instrumentation.ts`: Wraps better-sqlite3 prepared statements with OpenTelemetry client spans for statement tracking
- `packages/db/migrate.ts`: Runs database migrations via Drizzle ORM migrator unless degraded mode is enabled
- `packages/db/drizzle.config.ts`: Configuration file for Drizzle Kit schema generation and migration output directory

## Public interface
- db
- DB
- schema
- SqliteError
- KarakeepDBTransaction
- getInMemoryDB(runMigrations: boolean)
- openSqliteDatabase(filename: string, options: OpenSqliteOptions)
- instrumentDatabase(sqlite: Database.Database)

## Dependencies
- better-sqlite3
- drizzle-orm
- drizzle-kit
- @paralleldrive/cuid2
- @opentelemetry/api
- @karakeep/shared/config
- @karakeep/shared/logger
- @karakeep/shared/types/apiKeys
- @karakeep/shared/types/bookmarks

## Open questions
- packages/db/schema.ts is truncated in the provided file list; some table schemas and columns (like full bookmark schema definitions) are not fully visible.
