# fumadocs

**Type:** Open-source library (NOT a Noona-internal service)
**Language:** TypeScript
**Purpose:** Open-source React documentation framework supporting Next.js, Tanstack Start, Waku, and React Router. Published to npm. Used by noona-docs.

## Responsibilities
- Provide React UI components for documentation sites (`packages/ui`)
- MDX processing and plugin integration (`packages/mdx`, `packages/mdx-remote`)
- OpenAPI spec → documentation generation (`packages/openapi`)
- TypeScript API docs integration (`packages/typescript`)
- CLI tooling and project scaffolding (`packages/cli`, `packages/create-app`)

## Tech Stack
- **Monorepo:** Turborepo + pnpm workspaces
- **Build:** tsup (ESM-only packages)
- **Testing:** Vitest
- **Releases:** Changesets

## Integrations
- **noona-docs** — internal consumer of fumadocs packages

## Route here for
- Issues with the fumadocs framework itself (upstream open-source)
- Do NOT route Noona documentation content issues here — route those to noona-docs
