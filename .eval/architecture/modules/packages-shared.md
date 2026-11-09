# Module: packages/shared [AI]

(part 1 of 2) Provide shared utilities, schemas, and abstraction layers across the codebase, including configuration validation, bookmark import/export formats, AI prompt construction, LLM/embedding inference client factories, concurrency helpers, and plugin interfaces. (part 2 of 2) Provides core shared domain types, Zod schemas, validation logic, search query parsing, cryptographic token signing, and utility functions across Karakeep clients and backend services.

_This module does not fit in one model call, so it was read in 2 parts and their summaries were combined without a further model call._

## Key files
- `packages/shared/config.ts`: Defines and validates environment configurations using Zod schemas for inference, crawlers, authentication, embeddings, and queues.
- `packages/shared/inference.ts`: Implements inference and embedding clients (OpenAI and Ollama) with schema and dimension validations.
- `packages/shared/prompts.ts`: Constructs AI prompt templates for image/text tagging, summarization, and OCR extraction.
- `packages/shared/prompts.server.ts`: Server-side prompt building with token-budget calculation and content truncation via tiktoken.
- `packages/shared/plugins.ts`: Manages extensible plugin providers for asset stores, vector stores, queues, search indexes, and rate limiters.
- `packages/shared/queueing.ts`: Defines interfaces and types for job queues, worker runners, and queue plugins.
- `packages/shared/import-export/importer.ts`: Processes, stages, and converts parsed bookmark files into lists and bookmarks.
- `packages/shared/import-export/exporters.ts`: Transforms bookmarks and lists into standard Netscape HTML or JSON export formats.
- `packages/shared/import-export/parsers.ts`: Parses diverse bookmark import formats (Netscape HTML, Pocket, Matter, Karakeep, Omnivore, Linkwarden, etc.).
- `packages/shared/assetdb.ts`: Declares asset types, metadata schemas, and the AssetStore interface for binary asset persistence.
- `packages/shared/customFetch.ts`: Creates custom fetch instances with pooled Undici dispatchers and customizable timeouts/proxies.
- `packages/shared/concurrency.ts`: Implements AsyncSemaphore and limitConcurrency utilities for asynchronous task execution.
- `packages/shared/searchQueryParser.ts`: Implements parser combinator logic (via typescript-parsec) to parse user search query syntax into structured search matchers and filter ASTs.
- `packages/shared/search.ts`: Defines schemas, search document models, and the SearchIndexClient plugin interface for full-text search.
- `packages/shared/vectorStore.ts`: Defines vector document schemas and the VectorStoreClient plugin interface for semantic vector search and similarity lookups.
- `packages/shared/signedTokens.ts`: Utility functions for HMAC-SHA256 signing and schema-validated verification of time-aligned and expiring tokens.
- `packages/shared/ratelimiting.ts`: Defines rate limit configuration, identity resolution logic, and client interface specifications.
- `packages/shared/readOnlyMode.ts`: Determines mutation error messages for demo or degraded read-only modes.
- `packages/shared/storageQuota.ts`: Provides the QuotaApproved proof token class used during storage quota checks.
- `packages/shared/types/bookmarks.ts`: Core Zod schemas and TypeScript types defining bookmark payloads, assets, sources, and readable content formats.
- `packages/shared/types/rules.ts`: Zod definitions and validation logic for automation rules, triggers/events, nested conditions, and actions.
- `packages/shared/utils/highlight-anchoring.ts`: Algorithms for quote and context-based re-anchoring of text highlights across edited or re-crawled content.
- `packages/shared/utils/tag.ts`: Tag normalization and prompt generation helpers for AI-based automatic tagging and tag styling.

## Public interface
- InferenceClientFactory.build()
- EmbeddingClientFactory.build()
- OpenAIEmbeddingClient
- PluginManager (register, getClient, isRegistered, getPluginName, logAllPlugins)
- PluginType
- getQueueClient()
- QueueRetryAfterError
- queueOptionsEqual(left, right)
- buildImagePrompt(lang, customPrompts, tagStyle, curatedTags, potentialRelevantTags)
- constructTextTaggingPrompt(lang, customPrompts, content, tagStyle, curatedTags, potentialRelevantTags)
- constructSummaryPrompt(lang, customPrompts, content)
- buildTextPromptUntruncated(lang, customPrompts, content, tagStyle, curatedTags)
- buildSummaryPromptUntruncated(lang, customPrompts, content)
- buildOCRPrompt()
- buildTextPrompt(lang, customPrompts, content, contextLength, tagStyle, curatedTags, potentialRelevantTags)
- buildSummaryPrompt(lang, customPrompts, content, contextLength)
- importBookmarksFromFile(input, options)
- parseImportFile(source, textContent)
- toExportFormat(bookmark, listIds)
- toExportListFormat(list)
- toNetscapeFormat(bookmarks)
- zExportSchema
- zExportBookmarkSchema
- zExportListSchema
- zAssetMetadataSchema
- createCustomFetch(timeoutMs, proxyUrl)
- AsyncSemaphore
- limitConcurrency(promises, concurrencyLimit)
- tap(t, cb)
- debugPrint(t)
- throttledLogger(periodMs)
- parseSearchQuery(query: string): TextAndMatcher
- getRateLimitClient(): Promise<RateLimitClient | null>
- getRateLimitIdentity(opts: { userId?: string | null; ip?: string | null; internal?: boolean }): string | null
- getReadOnlyModeError(config: ReadOnlyModeConfig): string | null
- getSearchClient(): Promise<SearchIndexClient | null>
- getVectorStoreClient(): Promise<VectorStoreClient | null>
- createSignedToken(payload: unknown, secret: string, expiryEpoch?: number): string
- verifySignedToken<T>(token: string, secret: string, schema: z.ZodSchema<T>): T | null
- getAlignedExpiry(intervalSeconds: number, gracePeriodSeconds: number, now?: Date): number
- tryCatch<T, E = Error>(promise: Promise<T>): Promise<Result<T, E>>
- isAllowedBookmarkUrl(url: string): boolean
- validateRedirectUrl(url: string | null | undefined): string | undefined
- isMobileAppRedirect(url: string): boolean
- resolveHighlightRange(fullText: string, anchor: HighlightAnchor): ResolvedHighlightRange | null
- createHighlightResolver(fullText: string): (anchor: HighlightAnchor) => ResolvedHighlightRange | null
- getBookmarkDisplayTitle(bookmark: ZBookmark): string | null
- getBookmarkTitle(bookmark: ZBookmark): string | null
- getTextDisplayTitle(text: string, maxLength?: number): string | null
- getReadingPosition(container: HTMLElement): ReadingPosition | null
- scrollToReadingPosition(container: HTMLElement, offset: number, behavior?: ScrollBehavior, anchor?: string | null): boolean
- htmlToPlainText(htmlContent: string): string
- escapeHtml(input: string): string
- listsToTree(lists: ZBookmarkList[]): { allPaths: ZBookmarkList[][]; root: ZBookmarkListRoot; getPathById: (id: string) => ZBookmarkList[] | undefined }
- listNameFromPath(path: ZBookmarkList[]): string
- getTagStylePrompt(style: TagStyle): string
- getCuratedTagsPrompt(curatedTags?: string[]): string
- getPotentialRelevantTagsPrompt(potentialRelevantTags?: string[]): string
- normalizeTagName(raw: string): string
- QuotaApproved
- TRPC_MAX_URL_LENGTH_INTERNAL
- TRPC_MAX_URL_LENGTH_EXTERNAL

## Dependencies
- zod
- openai
- openai/helpers/zod
- ollama
- js-tiktoken
- cheerio
- csv-parse/sync
- undici
- winston
- typescript-parsec
- html-to-text
- node:crypto

## AI touchpoints [AI]
- `packages/shared/config.ts`
- `packages/shared/inference.test.ts`
- `packages/shared/inference.ts`
- `packages/shared/prompts.ts`
- `packages/shared/prompts.server.ts`
- `packages/shared/utils/tag.ts`
- `packages/shared/types/prompts.ts`

## Open questions
- _none_
