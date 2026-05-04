# Aient Docs

Mintlify documentation for Aient's public integration surface.

This repository is designed to build both:

- standalone in Mintlify Cloud from this directory; and
- as a generated submodule inside the Aient monorepo at `apps/aient-docs`.

## Local Preview

```bash
pnpm install
pnpm dev
```

## Validate

```bash
pnpm check
```

## Updating Generated Content

Webhook schema pages and generated navigation are owned by the Aient monorepo.
From the monorepo root, run:

```bash
pnpm build:aient-docs
pnpm test:aient-docs
pnpm check:aient-docs
```

Then commit the generated changes in this repository and update the monorepo
submodule pointer.
