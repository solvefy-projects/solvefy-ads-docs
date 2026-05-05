# SolvefyAds Embed — Documentação

Documentação pública do produto **SolvefyAds Embed** (integração via iframe
para parceiros white-label).

Site online: configurado via [Mintlify](https://mintlify.com).

## Estrutura

- `docs.json` — config do Mintlify (sidebar, tema, branding)
- `*.mdx` — páginas individuais (escritas em [MDX](https://mdxjs.com/))
- `logo/`, `favicon.svg`, `images/` — assets visuais
- Subpastas (`integration/`, `api-reference/`, `operators/`, `white-label/`)
  organizam grupos de páginas

## Desenvolvimento local

```bash
npx mintlify dev
```

Roda preview local em http://localhost:3000 (ou outra porta livre) com
hot-reload conforme você edita os `.mdx`.

## Deploy

Mintlify SaaS lê este repo direto via GitHub App e re-publica
automaticamente em cada push para `main`. URL final é configurada no painel
Mintlify (custom domain opcional).

## Editar conteúdo

Cada `.mdx` começa com frontmatter:

```mdx
---
title: "Título da página"
description: "Aparece no SEO e no preview da nav"
---

Conteúdo Markdown + componentes React (Card, CardGroup, Steps, Tabs, etc).
```

Componentes Mintlify disponíveis: <https://mintlify.com/docs/content/components>
