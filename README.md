# PhotonicsPowerLabs

**PhotonicsPowerLabs** is the primary umbrella repository for the Dotechin platform portfolio.  
It defines governance, standards, architecture boundaries, and cross-repository coordination for the following independent repositories:

- [UniqueItemTransferPlugin](https://github.com/dotechin/UniqueItemTransferPlugin)
- [CardsTradeMatcherPlugin](https://github.com/dotechin/CardsTradeMatcherPlugin)
- [TaskScheduler](https://github.com/dotechin/TaskScheduler)
- [ComplyFood](https://github.com/dotechin/ComplyFood)

> These repositories remain operationally and technically independent (separate codebases, releases, issues, CI/CD, and permissions), while being governed under one formal program structure.

---

## Program Objectives

- Establish a single source of truth for platform governance and standards.
- Ensure consistent security, quality, and release controls across all repos.
- Coordinate roadmap and integration touchpoints without forcing monorepo coupling.
- Preserve independent delivery velocity for each project.

---

## Repository Topology

This repository is a **meta-repo** (governance + documentation), not the deployment source for child projects.

See:
- [Repository Catalog](docs/repo-catalog.md)
- [Architecture Overview](docs/architecture.md)
- [Governance Model](docs/governance.md)
- [Security Policy](SECURITY.md)
- [Contribution Guide](CONTRIBUTING.md)

---

## Independence Model

Each child repository keeps:

- Its own issue tracker and pull requests
- Its own semantic versioning and releases
- Its own CI/CD workflows and runtime lifecycle
- Its own code ownership boundaries (aligned to shared standards)

PhotonicsPowerLabs provides:

- Shared policy and operating standards
- Cross-repo roadmap and dependency visibility
- Security and compliance baselines
- Program-level documentation

---

## Standardization Baseline (All Repos)

- Branch protection/rulesets on default branch
- Pull-request based changes (no direct push to protected branches)
- Required status checks
- Signed commits required
- Dependabot alerts + security updates
- Secret scanning + push protection
- CODEOWNERS and review ownership
- SECURITY.md and vulnerability reporting guidance

---

## Ownership & Authorization

Administrative and write access must be restricted to explicitly authorized maintainers only.  
Public visibility does **not** imply public write permissions.

See [Governance Model](docs/governance.md) for role definitions and enforcement.

---

## Quick Links

- **Primary repo:** [PhotonicsPowerLabs](https://github.com/dotechin/PhotonicsPowerLabs)
- **Sub-repos catalog:** [docs/repo-catalog.md](docs/repo-catalog.md)
- **Cross-repo change process:** [CONTRIBUTING.md](CONTRIBUTING.md)

---

## License

Unless otherwise specified, this repository’s content is licensed under the license declared in this repo.
