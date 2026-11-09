# Unique selling propositions

_Each USP is sourced to a business document (verbatim) and mapped to the components that deliver it._

## Self-hostable

The app can be hosted by users on their own infrastructure rather than depending on a vendor-run service.

- **Sources:**
  - `About_the_organisation.md`: "A self-hostable bookmark-everything app (links, notes and images) with AI-based automatic tagging and full text search"
- **Delivered by:** _no linked components_

## Bookmark everything

A single place to save links, notes and images, not just URLs.

- **Sources:**
  - `About_the_organisation.md`: "A self-hostable bookmark-everything app (links, notes and images) with AI-based automatic tagging and full text search"
- **Delivered by:** _no linked components_

## AI-based automatic tagging

Saved content is tagged automatically using AI, so users do not have to organise items by hand.

- **Sources:**
  - `About_the_organisation.md`: "A self-hostable bookmark-everything app (links, notes and images) with AI-based automatic tagging and full text search"
  - `About_the_organisation.md`: "AI-based automatic tagging and full text search"
- **Delivered by:**
  - `packages/shared/prompts::constructTextTaggingPrompt.prompt`, matched on named by the model while reading the business documents
  - `packages/shared/prompts::buildImagePrompt.prompt`, matched on named by the model while reading the business documents
  - `apps/web/components/settings/AISettings::AISettings`, matched on named by the model while reading the business documents
  - `apps/web/components/settings/AISettings::TaggingRules`, matched on named by the model while reading the business documents
  - `apps/web/components/settings/AISettings::TagStyleSelector`, matched on named by the model while reading the business documents
  - `apps/web/components/settings/AISettings::CuratedTagsSelector`, matched on named by the model while reading the business documents

## Full text search

Saved items are searchable by their full text content.

- **Sources:**
  - `About_the_organisation.md`: "A self-hostable bookmark-everything app (links, notes and images) with AI-based automatic tagging and full text search"
  - `About_the_organisation.md`: "AI-based automatic tagging and full text search"
- **Delivered by:** _no linked components_

## Coverage

- **Statements linked to code:** 2 of 8 · rule: 1/4 · usp: 1/4
- **Artifacts reached from the business:** 6 of 3412 linkable artifacts in the scan
- **How the links were made:** candidates from names, paths, routes and endpoints in your own code, confirmed by the model.

### Reach by area

- Web: 4 of 1172
- Mobile: 0 of 591
- Workers: 0 of 301
- Shared: 2 of 214
- Trpc: 0 of 198
- Browser extension: 0 of 145
- E2e tests: 0 of 120
- Cli: 0 of 98
- Plugins: 0 of 94
- Shared react: 0 of 91
- Tools: 0 of 69
- Landing: 0 of 67
- Shared server: 0 of 55
- Mcp: 0 of 50
- Api: 0 of 45
- Benchmarks: 0 of 30
- Open api: 0 of 18
- .agents: 0 of 17
- Db: 0 of 16
- Docs: 0 of 16
- Tooling: 0 of 3
- Sdk: 0 of 2

### Linked to nothing (6)

- **usp** Self-hostable: The only words that matched a name, path or route are too short to mean one thing (host, run, user), and a three- or four-letter stem matches by accident across two languages. Something longer has to match the same artifact.
- **usp** Bookmark everything: The only words that matched a name, path or route are too short to mean one thing (save), and a three- or four-letter stem matches by accident across two languages. Something longer has to match the same artifact.
- **usp** Full text search: 1 candidate(s) were offered and the model confirmed none of them.
- **rule** The app must be deployable as a self-hosted installation.: The only words that matched a name, path or route are too short to mean one thing (host), and a three- or four-letter stem matches by accident across two languages. Something longer has to match the same artifact.
- **rule** The app must support saving links, notes and images as bookmarkable items.: 1 candidate(s) were offered and the model confirmed none of them.
- **rule** Saved items must be discoverable through full text search.: The only words that matched a name, path or route are too short to mean one thing (item), and a three- or four-letter stem matches by accident across two languages. Something longer has to match the same artifact.

## Gaps

_None. All material was sourced._
