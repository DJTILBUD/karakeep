# Module: packages/shared-react

Provides shared React components, hooks, UI primitives, and context providers for managing bookmarks, reading progress, highlights, reader settings, tags, lists, search history, and tRPC API client integration across front-end applications.

## Key files
- `packages/shared-react/trpc.ts`: Exports the React Query tRPC context provider and hooks typed against AppRouter.
- `packages/shared-react/providers/trpc-provider.tsx`: Configures and initializes the tRPC HTTP batch client with SuperJSON serialization and React Query client provider.
- `packages/shared-react/providers/client-config-provider.tsx`: Provides runtime configuration context including auth, inference, chat, search, and crawler feature flags.
- `packages/shared-react/components/BookmarkHtmlHighlighter.tsx`: Renders desktop popover and touch/mobile dock interfaces for highlighting bookmark text and attaching notes.
- `packages/shared-react/components/ScrollProgressTracker.tsx`: Tracks viewport scroll progress on bookmark content, manages reading progress bars, and emits reading position snapshots.
- `packages/shared-react/hooks/bookmarks.ts`: React Query mutation and query hooks for bookmark retrieval, auto-refresh, CRUD, AI summarization, recrawling, and tagging.
- `packages/shared-react/hooks/reading-progress.ts`: Coordinates reading progress fetching, continue-reading banner state, scroll restoration, and position persistence.
- `packages/shared-react/hooks/reader-settings.tsx`: Manages typography settings with fallback precedence across session overrides, local device overrides, and server defaults.
- `packages/shared-react/hooks/query-invalidation.ts`: Debounces and schedules React Query invalidations to prevent redundant network refetches.

## Public interface
- TRPCSettingsProvider
- getTRPCClient
- useTRPC
- TRPCProvider
- ClientConfigProvider
- useClientConfig
- ScrollProgressTracker
- useReadingProgress
- useReaderSettings
- useAutoRefreshingBookmarkQuery
- useCreateBookmark
- useCreateBookmarkWithPostHook
- useUpdateBookmark
- useDeleteBookmark
- useSummarizeBookmark
- useRecrawlBookmark
- usePreserveOfflineCopy
- usePreserveBookmarkVideo
- useUpdateBookmarkTags
- useBookmarkPostCreationHook
- useCreateHighlight
- useUpdateHighlight
- useDeleteHighlight
- useBookmarkLists
- useCreateBookmarkList
- useEditBookmarkList
- useMergeLists
- useAddBookmarkToList
- useRemoveBookmarkFromList
- useDeleteBookmarkList
- usePaginatedSearchTags
- useTagAutocomplete
- useCreateTag
- useUpdateTag
- useMergeTag
- useDeleteTag
- useDeleteUnusedTags
- useSearchHistory
- useWhoAmI
- useUpdateUserSettings
- useUpdateUserProfile
- useUpdateUserAvatar
- useDeleteAccount
- useCreateRule
- useUpdateRule
- useDeleteRule
- useAttachBookmarkAsset
- useReplaceBookmarkAsset
- useDetachBookmarkAsset
- BookmarkGridContextProvider
- useBookmarkGridContext
- BookmarkListContextProvider
- useBookmarkListContext
- useDebounce
- scheduleInvalidateQueries
- Button
- Popover
- PopoverContent
- PopoverTrigger
- Textarea
- cn

## Dependencies
- @karakeep/shared
- @karakeep/trpc
- @radix-ui/react-popover
- @radix-ui/react-slot
- @tanstack/react-query
- @trpc/client
- @trpc/tanstack-react-query
- class-variance-authority
- clsx
- lucide-react
- react
- superjson
- tailwind-merge
- zod

## AI touchpoints [AI]
- `packages/shared-react/hooks/bookmarks.ts`
- `packages/shared-react/providers/client-config-provider.tsx`

## Open questions
- _none_
