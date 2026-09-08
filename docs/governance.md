# Governance Model

## 1) Purpose

This governance model establishes **PhotonicsPowerLabs** as the primary coordination repository and defines how independent repositories align on security, quality, and delivery practices.

## 2) Scope

Applies to:

- `dotechin/PhotonicsPowerLabs` (primary umbrella)
- `dotechin/UniqueItemTransferPlugin`
- `dotechin/CardsTradeMatcherPlugin`
- `dotechin/TaskScheduler`
- `dotechin/ComplyFood`

## 3) Repository Authority Model

- **Primary repo authority:** Program-level standards, architecture principles, cross-repo policy.
- **Sub-repo authority:** Implementation, testing, releases, local architecture decisions within policy boundaries.

## 4) Access Control Principles

1. Least privilege for all collaborators.
2. Public repos may be readable by all, but write/admin limited to authorized maintainers only.
3. Admin role should be rare and auditable.
4. Access reviews are mandatory and recurring.

## 5) Branch & Merge Policy (Minimum Baseline)

For default branch in every repo:

- Pull request required before merge
- At least 1 approval required (2 preferred for sensitive changes)
- Required status checks must pass
- Dismiss stale approvals on new commits
- Require signed commits
- Block force-push and branch deletion
- Restrict direct pushes to authorized maintainers/bots only

## 6) Security Baseline

Required in each repository:

- Dependabot alerts enabled
- Dependabot security updates enabled
- Secret scanning enabled
- Push protection for secrets enabled
- Code scanning enabled (CodeQL or equivalent)
- Private vulnerability reporting enabled (recommended)

## 7) Change Management

### 7.1 Policy Changes
- Open PR in `PhotonicsPowerLabs`
- Include rationale, impacted repos, rollout plan
- Require maintainer approval

### 7.2 Cross-Repo Changes
- Create tracking issue in primary repo
- Link implementation PRs in each affected sub-repo
- Define compatibility/version constraints explicitly

## 8) Release & Versioning

- Each sub-repo owns its own versioning and release cadence.
- Breaking changes impacting other repos must include:
  - migration notes
  - compatibility window
  - rollback plan

## 9) Compliance & Audit

- Monthly permission audit
- Monthly ruleset audit
- Quarterly security posture report
- Incident reviews documented in primary repo

## 10) Exception Process

Any exception to baseline policy must:
1. Be documented in writing
2. Include risk acceptance and expiration date
3. Be approved by repository admins
