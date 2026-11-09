# Module: tools/compare-models [AI]

Provides an interactive CLI benchmarking tool to compare AI automatic tagging performance either between two language models (model-vs-model) or between a candidate model and existing AI tags (model-vs-existing) on Karakeep bookmarks via blind A/B evaluation.

## Key files
- `tools/compare-models/src/index.ts`: CLI entry point coordinating bookmark retrieval, tag inference, randomized blind A/B presentation, user voting, and final tally reporting.
- `tools/compare-models/src/apiClient.ts`: API client wrapping @karakeep/sdk to fetch link bookmarks and existing tags from a Karakeep server instance.
- `tools/compare-models/src/bookmarkProcessor.ts`: Extracts text content from bookmark payloads and runs prompt generation and tag inference via shared utilities.
- `tools/compare-models/src/inferenceClient.ts`: Instantiates OpenAI inference clients and invokes structured text inference to parse generated tags.
- `tools/compare-models/src/config.ts`: Validates and parses environment variables for comparison settings, Karakeep credentials, and LLM parameters with Zod.
- `tools/compare-models/src/interactive.ts`: Terminal UI helper functions for interactive readline prompts, progress display, blind comparison layouts, and final scorecards.
- `tools/compare-models/src/types.ts`: TypeScript type declarations for bookmarks, model configurations, comparison votes, and final result summaries.

## Public interface
- KarakeepAPIClient.prototype.fetchBookmarks
- extractBookmarkContent
- runTaggingForModel
- createInferenceClient
- inferTags
- config
- askQuestion
- displayComparison
- displayError
- displayProgress
- clearProgress
- close
- displayFinalResults
- Bookmark
- ModelConfig
- ComparisonResult
- FinalResults

## Dependencies
- @karakeep/sdk
- @karakeep/shared/inference
- @karakeep/shared/prompts.server
- chalk
- zod
- node:readline

## AI touchpoints [AI]
- `tools/compare-models/src/bookmarkProcessor.ts`
- `tools/compare-models/src/inferenceClient.ts`
- `tools/compare-models/src/index.ts`

## Open questions
- _none_
