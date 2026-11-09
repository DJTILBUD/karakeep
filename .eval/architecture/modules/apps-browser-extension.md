# Module: apps/browser-extension

A browser extension (Chrome and Firefox) allowing users to save web pages, links, text selections, and images to their self-hosted or cloud Karakeep instance, edit titles, notes, tags, and lists, and perform client-side page snapshot capture using SingleFile.

## Key files
- `apps/browser-extension/src/background/background.ts`: Background service worker managing context menus, commands, tab URL lookups, and toolbar badge caching.
- `apps/browser-extension/src/main.tsx`: Extension popup entrypoint configuring providers and React Router routes.
- `apps/browser-extension/src/SavePage.tsx`: Popup view handling automatic or manual saving flows, SingleFile client-side capture coordination, and bookmark creation mutations.
- `apps/browser-extension/src/BookmarkSavedPage.tsx`: Post-save view facilitating bookmark deletion, title and note editing, and tag and list organization.
- `apps/browser-extension/src/content-scripts/singlefile-content-script.ts`: Content script injected into active tabs to generate complete HTML snapshots via single-file-core.
- `apps/browser-extension/src/utils/trpc.ts`: tRPC client and TanStack Query setup integrating Chrome storage cache persistence.
- `apps/browser-extension/src/utils/settings.ts`: Extension configuration and sync storage manager (server address, API keys, badge caching, auto-save, SingleFile settings).

## Public interface
- NEW_BOOKMARK_REQUEST_KEY_NAME: Storage session key used to pass bookmark requests between background script and popup
- CAPTURE_PAGE: Chrome runtime message handled by the SingleFile content script to capture page HTML
- MessageType.BOOKMARK_REFRESH_BADGE: Chrome runtime message triggering background tab badge status refresh

## Dependencies
- @karakeep/shared
- @karakeep/shared-react
- @karakeep/trpc
- @karakeep/tailwind-config
- single-file-core
- @tanstack/react-query
- @tanstack/react-query-persist-client
- @trpc/client
- react-router-dom
- @crxjs/vite-plugin
- lucide-react
- cmdk
- @radix-ui/react-dialog
- @radix-ui/react-popover
- @radix-ui/react-select
- @radix-ui/react-slot
- @radix-ui/react-switch
- zod

## AI touchpoints [AI]
- `apps/browser-extension/src/components/TagList.tsx`

## Open questions
- _none_
