# Guia Japão Incrível — MVP (PT/JA)

Bilingual (PT/JA) static website built with Astro and Tailwind. Focused on performance, SEO, and content‑driven pages.

## Estrutura
```
/
├── public/
│   ├── robots.txt
│   └── sitemap.xml
├── src/
│   ├── layouts/
│   │   └── Layout.astro
│   └── pages/
│       ├── index.astro          # redirect / → /pt/
│       ├── pt/
│       │   ├── index.astro      # Home (PT)
│       │   └── contato.astro    # Contact (PT)
│       └── ja/
│           ├── index.astro      # Home (JA)
│           └── contact.astro    # Contact (JA)
└── package.json
```

## Rotas
- `/` → redireciona para `/pt/`
- `/pt/`, `/pt/contato`
- `/ja/`, `/ja/contact`

## Convenções
- SSG‑first (Astro). Mínimo JS; ilhas somente quando necessário.
- Tailwind via `@tailwindcss/vite` (`src/styles/global.css`).
- `Layout.astro` define `lang`, `title`, `description` e alternates `hreflang` (`pt`, `ja`, `x-default`).

## SEO
- `lang` por página; títulos e descrições localizados.
- `robots.txt` e `sitemap.xml` estáticos (atualize o domínio em `public/sitemap.xml`).

## Comandos
- `npm install`
- `npm run dev` — http://localhost:4321
- `npm run build` — saída em `dist/`
- `npm run preview`

## Próximos passos
- Atualizar email de contato em: `src/pages/pt/contato.astro` e `src/pages/ja/contact.astro` (contact@example.com → seu email).
- Atualizar domínio no `public/sitemap.xml` (https://example.com → seu domínio).
