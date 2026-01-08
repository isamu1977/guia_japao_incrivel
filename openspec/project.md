# Project Context

## Purpose and Scope

Build and maintain a bilingual (PT/JA) content-driven website using Astro.
The site focuses on institutional pages, services, tours, and editorial content,
with lead generation as the primary goal.

The implementation must be lightweight, static-first, and optimized for SEO,
with minimal client-side JavaScript.

## Tech Stack and Constraints

- Astro 5.x (SSG-first; SSR only if explicitly approved).
- Tailwind CSS 4.x via `@tailwindcss/vite`.
- TypeScript with strict settings (`astro/tsconfigs/strict`).
- ESM modules only (`"type": "module"`).
- Package manager: bun. Do not use npm/yarn/pnpm commands in this repository. Use bun.
- No backend server or database in this repository.
- Static deployment (e.g. Cloudflare Pages).

## Language and Content Model

- Two languages with separate routes:
  - `/pt` for Portuguese
  - `/ja` for Japanese
- Content may differ by language.
- Content is stored as Markdown in the Git repository.
- Content types include:
  - Services
  - Tours
  - Blog posts / articles

## UI Direction

- Design style: premium minimalism.
- Typography-first layout with generous whitespace.
- Subtle borders and minimal shadows.
- No UI component library.
- Tailwind CSS utilities only.
- Mobile-first and accessible by default.

## Development Conventions

- Structure: `src/pages`, `src/components`, `src/layouts`, `src/content`, `public/`.
- Reusable Astro components for layout and UI primitives.
- Minimal JavaScript; Astro islands only when interaction is required.
- Avoid frontend frameworks (React/Vue/Svelte) unless explicitly justified.
- Small, focused commits and branches.

## Architectural Decisions

- Static Site Generation (SSG) as the default rendering model.
- Content driven by Markdown and build-time generation.
- Shared layouts and components across languages.
- No client-side routing as the primary navigation model.

## Non-Goals

- Backend APIs, authentication, or databases.
- Complex client-side state management.
- SPA-style application architecture.
- Heavy runtime dependencies or custom build pipelines.
