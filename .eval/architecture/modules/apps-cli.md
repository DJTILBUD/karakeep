# Module: apps/cli [AI]

Command-line interface (CLI) for Karakeep providing utilities to manage bookmarks, lists, tags, highlights, assets, user authentication, administration, data dumping, instance-to-instance migration, account wiping, and agent skill export.

## Key files
- `apps/cli/src/index.ts`: CLI entry point setting up global options, authentication checks, and Commander.js subcommands.
- `apps/cli/src/commands/bookmarks.ts`: Implements CLI commands for creating and manipulating link, text, and asset bookmarks.
- `apps/cli/src/commands/skill.ts`: Outputs the official Karakeep AI agent skill specification (SKILL.md).
- `apps/cli/src/commands/migrate.ts`: Facilitates full data migration between Karakeep servers including settings, lists, feeds, prompts, webhooks, tags, rules, and bookmarks.
- `apps/cli/src/commands/dump.ts`: Creates archived tar.gz exports of account data, settings, rules, prompts, bookmarks, and binary assets.
- `apps/cli/src/commands/wipe.ts`: Permanently deletes user data including bookmarks, lists, rules, feeds, prompts, and tags.
- `apps/cli/src/commands/admin.ts`: Admin management commands for user quotas, user deletion, stats, and bookmark debugging.
- `apps/cli/src/lib/trpc.ts`: Configures and instantiates tRPC clients for communication with the Karakeep backend.
- `apps/cli/src/lib/config.ts`: Handles reading, validating, and writing local CLI authentication configurations.
- `apps/cli/vite.config.mts`: Vite build configuration that bundles the Node.js CLI binary and inlines the agent skill definition.

## Public interface
- CLI command suite: admin, assets, auth, bookmarks, dump, highlights, lists, migrate, skill, tags, whoami, wipe
- getAPIClient(): tRPC client for the configured default Karakeep server
- getAPIClientFor(opts: { serverAddr: string; apiKey: string }): tRPC client for a specific target server
- loadConfig(): loads and normalizes CLI configuration from disk
- getConfigPath(): resolves the path to the user config file

## Dependencies
- @commander-js/extra-typings
- @karakeep/shared
- @karakeep/trpc
- @trpc/client
- chalk
- superjson
- table
- vite
- vite-tsconfig-paths
- zod

## AI touchpoints [AI]
- `apps/cli/src/commands/admin.ts`
- `apps/cli/src/commands/auth.ts`
- `apps/cli/src/commands/migrate.ts`
- `apps/cli/src/commands/wipe.ts`
- `apps/cli/src/commands/skill.ts`
- `apps/cli/src/commands/dump.ts`
- `apps/cli/src/commands/tags.ts`

## Open questions
- _none_
