# Guidelines

Conventions backed by **≥2** real, verbatim code examples. Anything with fewer is omitted below.

## Route/page-level React components are the default export of their file and are named after the file (e.g. SavePage.tsx exports `export default function SavePage()`); one page component per file.

- `apps/browser-extension/src/BookmarkDeletedPage.tsx`:

  ```
  export default function BookmarkDeletedPage() {
  ```

- `apps/browser-extension/src/BookmarkSavedPage.tsx`:

  ```
  export default function BookmarkSavedPage() {
  ```

- `apps/browser-extension/src/Layout.tsx`:

  ```
  export default function Layout() {
  ```

- `apps/browser-extension/src/OptionsPage.tsx`:

  ```
  export default function OptionsPage() {
  ```

- `apps/browser-extension/src/SavePage.tsx`:

  ```
  export default function SavePage() {
  ```

- `apps/browser-extension/src/ServerAddressPage.tsx`:

  ```
  export default function ServerAddressPage() {
  ```

## Reusable, non-page components are named exports declared as plain `function` components with props destructured and typed inline in the signature rather than via a separate props interface, unless the props are shared with a cva variant.

- `apps/browser-extension/src/components/ErrorCallout.tsx`:

  ```
  export function ErrorCallout({
  ```

- `apps/browser-extension/src/components/ListsSelector.tsx`:

  ```
  export function ListsSelector({ bookmarkId }: { bookmarkId: string }) {
  ```

- `apps/browser-extension/src/components/NoteEditor.tsx`:

  ```
  export function NoteEditor({ bookmarkId }: { bookmarkId: string }) {
  ```

- `apps/browser-extension/src/components/PopupHeader.tsx`:

  ```
  export function PopupHeader({
  ```

- `apps/browser-extension/src/components/StatusMessage.tsx`:

  ```
  export function StatusMessage({
  ```

- `apps/browser-extension/src/components/TagsSelector.tsx`:

  ```
  export function TagsSelector({ bookmarkId }: { bookmarkId: string }) {
  ```

- `apps/browser-extension/src/components/TitleEditor.tsx`:

  ```
  export function TitleEditor({ bookmarkId }: { bookmarkId: string }) {
  ```

## Components that render bookmark data take a `bookmarkId` prop and fetch the bookmark themselves (rather than receiving the full bookmark object), so each subcomponent stays independently refreshable.

- `apps/browser-extension/src/components/ListsSelector.tsx`:

  ```
  export function ListsSelector({ bookmarkId }: { bookmarkId: string }) {
  ```

- `apps/browser-extension/src/components/NoteEditor.tsx`:

  ```
  export function NoteEditor({ bookmarkId }: { bookmarkId: string }) {
  ```

- `apps/browser-extension/src/components/TagList.tsx`:

  ```
  export default function TagList({ bookmarkId }: { bookmarkId: string }) {
  ```

- `apps/browser-extension/src/components/TagsSelector.tsx`:

  ```
  export function TagsSelector({ bookmarkId }: { bookmarkId: string }) {
  ```

- `apps/browser-extension/src/components/TitleEditor.tsx`:

  ```
  export function TitleEditor({ bookmarkId }: { bookmarkId: string }) {
  ```

## Access the backend through the typed tRPC proxy from @karakeep/shared-react via `const api = useTRPC();` at the top of the component; do not instantiate ad-hoc fetch clients in UI code.

- `apps/browser-extension/src/SavePage.tsx`:

  ```
  const api = useTRPC();
  ```

- `apps/browser-extension/src/components/ListsSelector.tsx`:

  ```
  const api = useTRPC();
  ```

- `apps/browser-extension/src/components/TagsSelector.tsx`:

  ```
  const api = useTRPC();
  ```

## For live bookmark state (e.g. while crawling or AI tagging is still in progress) use the shared `useAutoRefreshingBookmarkQuery({ bookmarkId })` hook instead of a plain query so the UI polls until processing settles.

- `apps/browser-extension/src/components/NoteEditor.tsx`:

  ```
  const { data: bookmark } = useAutoRefreshingBookmarkQuery({ bookmarkId });
  ```

- `apps/browser-extension/src/components/TagList.tsx`:

  ```
  const { data: bookmark } = useAutoRefreshingBookmarkQuery({ bookmarkId });
  ```

## Hoist fixed strings, IDs, message keys and option tables to module-level `const` declarations in SCREAMING_SNAKE_CASE (or an uppercase object map) rather than inlining literals inside functions.

- `.agents/skills/fill-translations/i18n.mjs`:

  ```
  const REPO = execFileSync("git", ["rev-parse", "--show-toplevel"], {
  ```

- `.agents/skills/fill-translations/i18n.mjs`:

  ```
  const APPS = {
  ```

- `apps/browser-extension/src/OptionsPage.tsx`:

  ```
  const THEME_OPTIONS = [
  ```

- `apps/browser-extension/src/SignInPage.tsx`:

  ```
  const CONNECTION_ERROR_MESSAGE =
  ```

- `apps/browser-extension/src/background/background.ts`:

  ```
  const OPEN_KARAKEEP_ID = "open-karakeep";
  ```

- `apps/browser-extension/src/background/background.ts`:

  ```
  const ADD_LINK_TO_KARAKEEP_ID = "add-link";
  ```

- `apps/browser-extension/src/background/protocol.ts`:

  ```
  export const NEW_BOOKMARK_REQUEST_KEY_NAME = "karakeep-new-bookmark";
  ```

## Build small UI primitives (badge, button) with class-variance-authority: declare a `xxxVariants = cva(...)` constant and derive the component props from it, following the shadcn/ui pattern shared across the clients.

- `apps/browser-extension/src/components/ui/badge.tsx`:

  ```
  const badgeVariants = cva(
  ```

- `apps/browser-extension/src/components/ui/badge.tsx`:

  ```
  export interface BadgeProps
  ```

- `apps/browser-extension/src/components/ui/button.tsx`:

  ```
  const buttonVariants = cva(
  ```

## Presentational leaf components accept an optional `className?: string` prop so callers can compose Tailwind classes without wrapping the element.

- `apps/browser-extension/src/Logo.tsx`:

  ```
  export default function Logo({ className }: { className?: string }) {
  ```

- `apps/browser-extension/src/Spinner.tsx`:

  ```
  export default function Spinner({ className }: { className?: string }) {
  ```

## In the browser extension popup, navigate between screens with react-router's `useNavigate()` hook obtained at the top of the component instead of manipulating window.location.

- `apps/browser-extension/src/Layout.tsx`:

  ```
  const navigate = useNavigate();
  ```

- `apps/browser-extension/src/ServerAddressPage.tsx`:

  ```
  const navigate = useNavigate();
  ```
