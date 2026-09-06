# Repository Catalog

This catalog defines the formal relationship between the **primary umbrella repo** and associated independent repositories.

## Primary (Umbrella) Repository

| Repository | Role | Purpose |
|---|---|---|
| [dotechin/PhotonicsPowerLabs](https://github.com/dotechin/PhotonicsPowerLabs) | Primary / Umbrella | Governance, standards, architecture boundaries, program documentation, cross-repo coordination |

## Independent Sub-Repositories

| Repository | Domain Focus | Independence Status | Notes |
|---|---|---|---|
| [dotechin/UniqueItemTransferPlugin](https://github.com/dotechin/UniqueItemTransferPlugin) | Plugin / item transfer capabilities | Independent | Own codebase, issues, CI/CD, release cycle |
| [dotechin/CardsTradeMatcherPlugin](https://github.com/dotechin/CardsTradeMatcherPlugin) | Plugin / trade matching capabilities | Independent | Own codebase, issues, CI/CD, release cycle |
| [dotechin/TaskScheduler](https://github.com/dotechin/TaskScheduler) | Task orchestration & scheduling | Independent | Own codebase, issues, CI/CD, release cycle |
| [dotechin/ComplyFood](https://github.com/dotechin/ComplyFood) | Compliance/domain application | Independent | Own codebase, issues, CI/CD, release cycle |

---

## Relationship Rules

1. **No hidden coupling:** Sub-repos must not rely on undocumented internal behavior of each other.
2. **Contract-first integration:** Any cross-repo dependency must be documented with versioned contracts/interfaces.
3. **Independent release authority:** Each sub-repo can release independently.
4. **Shared policy, local execution:** Global standards are set by PhotonicsPowerLabs; implementation remains local per repo.
5. **Security baseline required:** All repos must meet minimum branch protection and security controls.

---

## Change Classification

Use this matrix to decide where changes belong:

| Change Type | Primary Repo (PhotonicsPowerLabs) | Sub-Repo |
|---|---|---|
| Governance/policy updates | ✅ | ❌ |
| Architecture documentation | ✅ | ⚠️ (local details only) |
| Feature implementation | ❌ | ✅ |
| Repo-specific CI/CD | ❌ | ✅ |
| Cross-repo standards | ✅ | ✅ (adoption) |
| Incident/postmortem summary | ✅ | ✅ (technical details) |

---

## Maintenance Cadence

- **Monthly:** Access review (admins/writers/collaborators)
- **Monthly:** Branch protection/ruleset compliance check
- **Quarterly:** Security baseline review across all repos
- **Quarterly:** Catalog and ownership metadata refresh