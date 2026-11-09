# Module: packages/sdk

Provides a typed API client SDK for interacting with the Karakeep backend API using openapi-fetch and generated TypeScript schema definitions.

## Key files
- `packages/sdk/src/index.ts`: Exports the typed client factory functions createKarakeepClient and createHoarderClient along with API schema types.
- `packages/sdk/src/karakeep-api.d.ts`: Contains generated OpenAPI path and component type definitions for the API.
- `packages/sdk/vite.config.mts`: Configures the Vite build to bundle the SDK for ES and CommonJS module formats.

## Public interface
- createKarakeepClient
- createHoarderClient
- type KarakeepAPISchemas

## Dependencies
- openapi-fetch
- vite
- vite-tsconfig-paths

## Open questions
- _none_
