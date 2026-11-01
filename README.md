# bcd-Aegora — Organization GitHub Defaults

Organization-wide GitHub contribution policies, community templates, and the org profile README.

## Repositories

- Product and architecture documentation: [`aegora-docs`](https://github.com/bcd-Aegora/aegora-docs)
- Backend: [`aegora-backend`](https://github.com/bcd-Aegora/aegora-backend)
- Frontend: [`aegora-frontend`](https://github.com/bcd-Aegora/aegora-frontend)
- Smart contracts: [`aegora-contracts`](https://github.com/bcd-Aegora/aegora-contracts)
- This repo (`.github`): org profile, default issue/PR templates, CONTRIBUTING, SECURITY, governance

## What belongs here

- `profile/README.md` — organization profile
- Root community health files (`CONTRIBUTING.md`, `SECURITY.md`, …) — defaults for repos that do not define their own
- `.github/ISSUE_TEMPLATE/` and `.github/PULL_REQUEST_TEMPLATE.md` — default issue/PR forms
- `GOVERNANCE.md` — team engineering governance (human-facing; not auto-enforced by GitHub)

## What does **not** belong here

- Application source, PRDs, ADRs, or Solidity
- Per-repo CI workflows — live in each product repository
- Per-repo `CODEOWNERS` — path owners belong in `aegora-backend`, `aegora-frontend`, `aegora-contracts`, etc.

Deep engineering workflow lives in [`aegora-docs/engineering`](https://github.com/bcd-Aegora/aegora-docs/tree/main/engineering). Keep this repository thin and GitHub-facing.
