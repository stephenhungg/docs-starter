# Documentation project instructions

This repository is the published Mintlify site for Hyper. Pages are MDX with YAML frontmatter
and configuration lives in `docs.json`.

## Where content comes from

Pages under `api/` are generated from the Markdown specs in the product repo by `docs/sync.py`.
Editing them here is a dead end: the next sync overwrites the change. Fix the spec in the
product repo instead and re-run the generator.

The four guides at the root — `index`, `architecture`, `mcp`, `deployment` — are written by hand
and are edited here.

## Conventions

- Say what the system does, not what it is going to do. Describe behaviour that exists.
- An API page documents the route, its authorization, and what the caller is responsible for.
- Code samples must be runnable as written. No placeholder hostnames where a real one is known.
- Link with root-relative paths (`/api/accounting`), never `.md` file paths — those 404 once
  Mintlify renders them.
