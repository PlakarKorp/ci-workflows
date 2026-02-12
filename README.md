# ci-workflows

It hosts **reusable workflows** that other repositories can call to run
consistent CI jobs (build/test/lint/release/deploy) without duplicating YAML
across (too) many repositories.

It guarantees:

- a **single source of truth** for CI logic,
- **consistent defaults** (runners, caching, permissions, artifacts),
- **safer changes** via versioned tags (`v1`, `v2`, ...),
- **lightweight per-repository workflows** (just a wrapper that calls the
  shared workflow)
