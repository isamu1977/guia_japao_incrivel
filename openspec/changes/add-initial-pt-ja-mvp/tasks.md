## 1. Implementation

- [ ] 1.1 Create locale directories `src/pages/pt/` and `src/pages/ja/`
- [ ] 1.2 Add Home pages (`index.astro`) for PT and JA with localized copy
- [ ] 1.3 Add Contact pages (`contato.astro` for PT, `お問い合わせ.astro` or `contact.astro` for JA) with mailto link
- [ ] 1.4 Implement global layout with `<html lang>` per locale and shared header/footer
- [ ] 1.5 Add language switcher linking to equivalent localized path
- [ ] 1.6 Add per-locale `<title>` and `<meta name="description">`
- [ ] 1.7 Add `robots.txt` and `sitemap.xml` (static or Astro integration if approved)
- [ ] 1.8 Validate: build locally, verify routes `/pt/*` and `/ja/*`, check Lighthouse basics
- [ ] 1.9 Update README with structure and commands

## 2. QA / Acceptance
- [ ] 2.1 PT and JA pages render with correct `lang` attribute
- [ ] 2.2 Language switcher navigates between PT and JA equivalents
- [ ] 2.3 Titles and descriptions are localized
- [ ] 2.4 Sitemap lists both locale paths; robots present
- [ ] 2.5 No console errors; Lighthouse passes basic SEO/performance checks
