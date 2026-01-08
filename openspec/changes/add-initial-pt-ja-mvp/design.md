## Context
Minimal bilingual static site (PT/JA) using Astro (SSG-first) and Tailwind. No backend, CMS, or SPA routing.

## Goals / Non-Goals
- Goals: PT/JA pages (Home, Contact), shared layout, switcher, SEO basics
- Non-Goals: CMS, blog, booking, payments, auth, backend services

## Decisions
- Locale strategy: path prefixes `/pt/*` and `/ja/*` for simplicity and clarity
- Root path: `/` redirects to `/pt/`
- Content placement: duplicate per-locale pages under `src/pages/{pt,ja}/`
- JA contact path: use `/ja/contact` for the MVP
- Switcher: static link to matching path; no runtime i18n framework
- SEO: set `<html lang>`, localized titles/descriptions; provide sitemap/robots (static acceptable)
- SEO alternates: add minimal `rel="alternate" hreflang` for `pt`, `ja`, and `x-default`
- Performance: minimal JS; images optimized and lazy by default

## Risks / Trade-offs
- Duplicate content across locales (no shared CMS) → simple to ship; manual sync
- Path-based locale with two trees → clear URLs; minor duplication

## Migration Plan
1. Create per-locale page trees
2. Implement layout and switcher
3. Add SEO meta, hreflang alternates, and static sitemap/robots
4. Validate and iterate on copy

## Open Questions
- Canonical/alternate link strategy depth: restrict to minimal alternates for MVP (decided), expand later?
