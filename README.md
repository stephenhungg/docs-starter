# Hyper documentation

The published documentation for [Hyper](https://hyper.stephenhung.me) — accounts payable that
shows its work. Deployed by Mintlify from `main`.

## Layout

- `index.mdx`, `architecture.mdx`, `mcp.mdx`, `deployment.mdx` — the guides
- `api/*.mdx` — one page per backend surface
- `docs.json` — navigation, theme and site config

## Editing

The API pages are generated from the Markdown specs in the product repo
(`backend/*.md`) by `docs/sync.py` there, so an API change updates the docs in the same commit
that makes it. Edit those specs rather than the generated pages; the guides are written by hand
and can be edited directly here.
