# Evaluation knowledge base: karakeep

Additive, grounded documentation produced as PR #0. No existing code was modified beyond inserting
comment identifiers; everything else lives here under `.eval/`, apart from the files listed under
"Outside .eval/".

## Contents (46 file(s) added)

- [`CLAUDE.md`](CLAUDE.md): Repo-specific orientation for AI agents (build, identifiers, conventions).
- [`INDEX.md`](INDEX.md): This index: every file this pull request adds.
- [`architecture/Architecture.md`](architecture/Architecture.md): System overview, module table (with [AI] markers), dependency graph.
- [`architecture/guidelines.md`](architecture/guidelines.md): Coding conventions, each backed by ≥2 verbatim code examples.
- [`architecture/modules/agents-skills.md`](architecture/modules/agents-skills.md): Summary of the `agents-skills` module, with the files it names.
- [`architecture/modules/apps-browser-extension.md`](architecture/modules/apps-browser-extension.md): Summary of the `apps-browser-extension` module, with the files it names.
- [`architecture/modules/apps-cli.md`](architecture/modules/apps-cli.md): Summary of the `apps-cli` module, with the files it names.
- [`architecture/modules/apps-landing.md`](architecture/modules/apps-landing.md): Summary of the `apps-landing` module, with the files it names.
- [`architecture/modules/apps-mcp.md`](architecture/modules/apps-mcp.md): Summary of the `apps-mcp` module, with the files it names.
- [`architecture/modules/apps-mobile.md`](architecture/modules/apps-mobile.md): Summary of the `apps-mobile` module, with the files it names.
- [`architecture/modules/apps-web.md`](architecture/modules/apps-web.md): Summary of the `apps-web` module, with the files it names.
- [`architecture/modules/apps-workers.md`](architecture/modules/apps-workers.md): Summary of the `apps-workers` module, with the files it names.
- [`architecture/modules/docs-docs.md`](architecture/modules/docs-docs.md): Summary of the `docs-docs` module, with the files it names.
- [`architecture/modules/docs-src.md`](architecture/modules/docs-src.md): Summary of the `docs-src` module, with the files it names.
- [`architecture/modules/docs-versioned-docs.md`](architecture/modules/docs-versioned-docs.md): Summary of the `docs-versioned-docs` module, with the files it names.
- [`architecture/modules/docs.md`](architecture/modules/docs.md): Summary of the `docs` module, with the files it names.
- [`architecture/modules/packages-api.md`](architecture/modules/packages-api.md): Summary of the `packages-api` module, with the files it names.
- [`architecture/modules/packages-benchmarks.md`](architecture/modules/packages-benchmarks.md): Summary of the `packages-benchmarks` module, with the files it names.
- [`architecture/modules/packages-db.md`](architecture/modules/packages-db.md): Summary of the `packages-db` module, with the files it names.
- [`architecture/modules/packages-e2e-tests.md`](architecture/modules/packages-e2e-tests.md): Summary of the `packages-e2e-tests` module, with the files it names.
- [`architecture/modules/packages-open-api.md`](architecture/modules/packages-open-api.md): Summary of the `packages-open-api` module, with the files it names.
- [`architecture/modules/packages-plugins.md`](architecture/modules/packages-plugins.md): Summary of the `packages-plugins` module, with the files it names.
- [`architecture/modules/packages-sdk.md`](architecture/modules/packages-sdk.md): Summary of the `packages-sdk` module, with the files it names.
- [`architecture/modules/packages-shared-react.md`](architecture/modules/packages-shared-react.md): Summary of the `packages-shared-react` module, with the files it names.
- [`architecture/modules/packages-shared-server.md`](architecture/modules/packages-shared-server.md): Summary of the `packages-shared-server` module, with the files it names.
- [`architecture/modules/packages-shared.md`](architecture/modules/packages-shared.md): Summary of the `packages-shared` module, with the files it names.
- [`architecture/modules/packages-trpc.md`](architecture/modules/packages-trpc.md): Summary of the `packages-trpc` module, with the files it names.
- [`architecture/modules/tooling-tailwind.md`](architecture/modules/tooling-tailwind.md): Summary of the `tooling-tailwind` module, with the files it names.
- [`architecture/modules/tools-compare-models.md`](architecture/modules/tools-compare-models.md): Summary of the `tools-compare-models` module, with the files it names.
- [`architecture/modules/tools-seed-snapshot.md`](architecture/modules/tools-seed-snapshot.md): Summary of the `tools-seed-snapshot` module, with the files it names.
- [`business/BusinessRules.md`](business/BusinessRules.md): Business rules, sourced, marked verifiable (yes/no), linked to @uxid.
- [`business/USPs.md`](business/USPs.md): Unique selling propositions, sourced to docs, mapped to @uxid.
- [`design-system/components.md`](design-system/components.md): The component inventory: every @uxid with its file, flow and type, coverage per flow, then each component’s variant axes, values and states.
- [`design-system/design.json`](design-system/design.json): The whole extracted design system as one record: theme sources, token groups, scales, component variants, composition, disagreements.
- [`design-system/kit.json`](design-system/kit.json)
- [`design-system/playbook.html`](design-system/playbook.html): The design system as one self-contained page. Open it from the checkout; nothing serves it.
- [`design-system/playbook.md`](design-system/playbook.md): The readable playbook: where the theme is declared, the palette and scales, the primitives, and where the app disagrees with itself.
- [`design-system/tokens.json`](design-system/tokens.json): Design tokens: role, family, light/dark pair, utility name, usage count, and every declaration site.
- [`design-system/tokens.md`](design-system/tokens.md): The token catalogue, grouped by the job each token does.
- [`design-system/typography.json`](design-system/typography.json): Fonts, @font-face rules and the type scale, as declared.
- [`knowledge/company.md`](knowledge/company.md): What the company is and sells, in its own sourced words.
- [`knowledge/customers.md`](knowledge/customers.md): Who uses the product, and the outcome each segment came for.
- [`knowledge/glossary.md`](knowledge/glossary.md): Terms the company uses in a specific way, as its material defines them.
- [`knowledge/goals.md`](knowledge/goals.md): What "good" means to this company, each goal with its source.
- [`pipeline.yaml`](pipeline.yaml): Detected stack, the install/build/analyze/test commands, and whether each was run.
- [`product-map.json`](product-map.json): The product in four floors: pages, API actions, the code doing the work, its data.
