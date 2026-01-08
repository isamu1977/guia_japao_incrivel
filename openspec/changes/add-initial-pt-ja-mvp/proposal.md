# Change: Initial website MVP (PT/JA)

## Why
Deliver the first public, bilingual (PT/JA) marketing site for a premium Japan tourism and guide service, focusing on performance, SEO, and content-driven pages with minimal complexity.

## What Changes
- Add site shell (shared layout, header, footer)
- Add PT/JA localization using path-based routes and language switcher
- Add root path redirect: `/` → `/pt/`
- Add core pages: Home and Contact in PT and JA
- Add SEO basics: lang attribute, per-locale titles/descriptions, hreflang alternates (pt, ja, x-default), sitemap and robots

## Impact
- Affected specs: site-shell, i18n, pages-core, seo-basics
- Affected code (indicative): `src/layouts/Layout.astro`, `src/pages/pt/*`, `src/pages/ja/*`, navigation/header component, static files under `public/`

## Out of Scope (for this change)
- CMS or dynamic content management
- Blog, booking flows, or payments
- Authentication or user accounts
- Backend services or databases
