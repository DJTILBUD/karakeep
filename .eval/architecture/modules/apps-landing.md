# Module: apps/landing [AI]

Provides the public marketing, documentation links, application directory, pricing, legal pages, and pricing markdown API for Karakeep using Astro and React.

## Key files
- `apps/landing/astro.config.ts`: Configures Astro static site generation, React integration, sitemap alias hook, and Vite plugins
- `apps/landing/src/Homepage.tsx`: Main landing page assembling platform links, use cases, LLM-ready features, and call-to-action sections
- `apps/landing/src/Apps.tsx`: Presents available clients including mobile apps, browser extensions, community integrations, and agentic skills
- `apps/landing/src/Pricing.tsx`: Interactive pricing tier matrix with monthly/yearly toggles, feature breakdowns, and FAQ section
- `apps/landing/src/pricing-data.ts`: Source of truth for pricing tier definitions, feature lists, savings calculations, and FAQ entries
- `apps/landing/src/pages/pricing.md.ts`: Astro API route serving structured markdown output of pricing information at /pricing.md

## Public interface
- GET /pricing.md (APIRoute serving markdown-formatted pricing details)
- default export Homepage() (React page component)
- default export Apps() (React page component)
- default export Pricing() (React page component)
- default export NavBar() (React navigation component)
- default export Footer() (React footer component)
- default export PrivacyPolicy() (React legal page component)
- default export Terms() (React terms page component)

## Dependencies
- astro
- @astrojs/react
- @astrojs/sitemap
- @karakeep/tailwind-config
- @radix-ui/react-slot
- class-variance-authority
- clsx
- lucide-react
- tailwind-merge
- vite-plugin-svgr

## AI touchpoints [AI]
- `apps/landing/src/Privacy.tsx`

## Where the code disagrees with the stack profile
- `apps/landing/astro.config.ts`: apps/landing is built using Astro with @astrojs/react rather than an unrecognised framework.

## Open questions
- _none_
