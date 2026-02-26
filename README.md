# fumadocs

> Open-source documentation framework for React.js — supports Next.js, Tanstack Start, Waku, and React Router.

---

## Overview

A monorepo for Fumadocs — an open-source documentation framework for React.js applications, supporting Next.js, Tanstack Start, Waku, and React Router.

## Tech Stack

- **Language:** TypeScript
- **Monorepo tooling:** Turborepo + pnpm workspaces
- **Build:** tsup
- **Testing:** Vitest
- **Target runtimes:** React.js (Next.js, Vite-based: Tanstack Start, Waku, React Router)
- **Packages:** ESM-only

## Architecture / How it works

Organized as a monorepo with `packages/` and `apps/`:

**Core packages:**
- `packages/core` — core logic and utilities
- `packages/ui` — React UI components for documentation pages
- `packages/mdx` — MDX processing and plugin integration
- `packages/mdx-remote` — remote MDX loading support
- `packages/openapi` — OpenAPI spec to docs generation
- `packages/typescript` — TypeScript API docs integration
- `packages/twoslash` — TwoSlash code annotation support
- `packages/content-collections` — content collections integration
- `packages/cli` — CLI tooling
- `packages/create-app` — project scaffolding

**Apps:**
- `apps/docs` — the Fumadocs documentation site itself

Releases are managed via Changesets. All packages are ESM-only.

## Key Interfaces / API

Fumadocs exposes React components, MDX plugins, and utilities distributed as npm packages. `packages/ui` exports the component library; `packages/core` exports routing and data utilities. Consumers install individual packages from npm.

## Dependencies

Standalone open-source library — no dependencies on other Noona services.
