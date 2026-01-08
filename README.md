# Brasil Logic Monorepo

Monorepo com **Turborepo** + **pnpm workspaces** no modelo Hub-and-Spoke.

- **Spokes (`apps/`)** — aplicações finais
- **Hub (`packages/`)** — configs e código compartilhado

## Estrutura

```
apps/
└── web                    # Next.js 16 (App Router)

packages/
├── config-biome           # Configuração Biome (lint/format)
├── config-tailwind        # Design tokens Tailwind CSS v4
└── config-typescript      # tsconfig compartilhado
```

## Requisitos

- **Node.js** ≥ 20 (com Corepack)
- **pnpm** ≥ 10

Ativar o Corepack (uma vez):

```bash
corepack enable
```

## Comandos

| Comando           | Descrição                   |
| ----------------- | --------------------------- |
| `pnpm install`    | Instala dependências        |
| `pnpm dev`        | Inicia dev server           |
| `pnpm build`      | Build de produção           |
| `pnpm lint`       | Lint com Biome              |
| `pnpm format`     | Formata código              |
| `pnpm type-check` | Verifica tipos TypeScript   |
| `pnpm clean`      | Limpa caches e node_modules |

## Stack

- **Next.js 16** — Framework React
- **Tailwind CSS v4** — Styling (CSS-first config)
- **Biome** — Linting e formatting
- **Turborepo** — Build system
- **pnpm** — Package manager
