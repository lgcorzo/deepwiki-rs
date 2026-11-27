# Architecture: `deepwiki-rs` in Dark Gravity

## Ecosystem Role & Tier

- **Tier**: `maintained_fork` (`MAINTAINED_FORK_PROFILE`, upstream `sopaco/deepwiki-rs`)
- **Role**: Rust Tree-sitter AST comprehension engine and Orphan Symbol Rate (`OSR < 5%`) verification tool validating generated OKF wikis and architecture diagrams across Dark Gravity repositories.
- **Visibility**: `public`

## Internal Component Design

Preserves the upstream Rust crate layout (`Cargo.toml`, `src/`, `skills/`, `docs/`, `UPSTREAM_AND_FORK_POLICY.md`) for clean Tree-sitter structural parsing across Rust, Python, and Go targets while normalizing lowercase `AGENTS.md` discovery on Linux systems.

## Upstream & Downstream Ecosystem Interfaces

```text
Target Dark Gravity Repos ──► deepwiki-rs (Tree-sitter AST + OSR < 5% check)
                                 ├──► DocumentationAgent (ISO 42010 / OKF Wiki synthesis)
                                 └──► R2R v3 Engine (indexed structural chunks)
```

## Security Boundary & Governance

- **`MAINTAINED_FORK_PROFILE` & Vertex 4 HITL**: Keeps upstream structure and license intact, omits `upstream` remote, and routes all patches through human-reviewed PRs (`DOC-011` compliant).

## Canonical Cross-Links

- [DARK_GRAVITY_MANIFEST.md](./DARK_GRAVITY_MANIFEST.md)
- [REPOSITORIES.md](./REPOSITORIES.md)
- [Global Architecture Portal](https://lgcorzo.github.io/architecture.html)
- [Unified Start-Here Portal](https://lgcorzo.github.io/start-here)
- [AI Auditor Pack](https://lgcorzo.github.io/docs/auditor/)
