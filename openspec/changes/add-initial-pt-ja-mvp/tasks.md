## 1. Implementation

- [x] 1.1 Create locale directories `src/pages/pt/` and `src/pages/ja/`
- [x] 1.2 Add Home pages (`index.astro`) for PT and JA with localized copy
- [x] 1.3 Add Contact pages (`contato.astro` for PT, `contact.astro` for JA) with mailto link
- [x] 1.4 Implement global layout with `<html lang>` per locale and shared header/footer
- [x] 1.5 Add language switcher linking to equivalent localized path
- [x] 1.6 Add per-locale `<title>` and `<meta name="description">`
- [x] 1.7 Add `robots.txt` and `sitemap.xml` (static)
- [x] 1.8 Validate: build locally, verify routes `/pt/*` and `/ja/*`, check Lighthouse basics
- [ ] 1.9 Update README with structure and commands

## 2. QA / Acceptance
- [x] 2.1 PT and JA pages render with correct `lang` attribute
- [x] 2.2 Language switcher navigates between PT and JA equivalents
- [x] 2.3 Titles and descriptions are localized
- [x] 2.4 Sitemap lists both locale paths; robots present
- [ ] 2.5 No console errors; Lighthouse passes basic SEO/performance checks
