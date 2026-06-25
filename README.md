# Registry Docs

**Moved:** Active development has moved to the public monorepo:
[`registrystack/registry-stack`](https://github.com/registrystack/registry-stack).

This repository is retained for pre-monorepo history and release tags. File new
issues and pull requests in the monorepo.

Current source at monorepo ref `ab5a1d46df8715539f15d398804611e8ca9c52d9`:

- [`docs/site/`](https://github.com/registrystack/registry-stack/tree/ab5a1d46df8715539f15d398804611e8ca9c52d9/docs/site)

**Legacy status:** Current documentation development happens in the monorepo.

Registry Docs is the canonical documentation website for the registry project
family.

It explains the map: which project owns which responsibility, which standards
claims are supported by evidence, which machine contracts are stable enough for
integrators, how Registry Notary federation fits into the stack, and how to run
the smallest end-to-end demo.

## Develop

```sh
npm install
npm run dev
```

## Validate

```sh
npm run check
```

The check command validates frontmatter, generated data, Markdown structure,
prose style, OpenAPI snapshots, SVG accessibility, Astro types, the static
build, and generated Redoc API pages.

## Content Sources

Data-backed reference tables are generated from:

- `src/data/projects.yaml`
- `src/data/contracts.yaml`
- `src/data/standards.yaml`
- `src/data/openapi-sources.yaml`

Run `npm run generate` after editing these files.
