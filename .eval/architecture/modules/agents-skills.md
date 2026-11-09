# Module: .agents/skills

Provides CLI utilities and skills for automated workflows/agents to audit, compare, and merge internationalization (i18n) translation keys across web and mobile locales against the English source of truth using git history.

## Key files
- `.agents/skills/fill-translations/i18n.mjs`: CLI tool that analyzes git commit history to detect missing, outdated, and obsolete translation strings across locales, and applies translations back into JSON locale files.

## Public interface
- node .agents/skills/fill-translations/i18n.mjs report [--app web|mobile] [--locales <locales>] [--json]
- node .agents/skills/fill-translations/i18n.mjs apply [--app web|mobile] <locale> <file.json> [--prune]

## Dependencies
- node:child_process
- node:fs
- node:path

## Open questions
- Are there other translation skills or agent definitions associated with this directory that were not included in the source snapshot?
