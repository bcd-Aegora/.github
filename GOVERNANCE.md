# bcd-Aegora Team Engineering Governance — v2

## Protected branches

- Protect `main` on `aegora-frontend`, `aegora-backend`, `aegora-contracts`, and `aegora-docs`.
- Require PRs, green checks, resolved conversations and at least one human reviewer.
- Require CODEOWNERS on policies, payments, contracts, authentication and deployment where feature access/plan supports.
- Do not enable self-approval of sensitive changes or direct AI merges.
- Never run privileged deployment jobs for untrusted pull-request code.

## One organization project

Fields: Status (Backlog, Ready, In Progress, In Review, Verified, Done), Priority, Area, Owner, Iteration, Risk, Release, Cross-repo dependency.

## AI authoring policy

- Agent code is normal code and must meet tests/security/review rules.
- Never let the agent disable checks, delete tests or relax security gates merely to pass CI.
- Keep MCP tools least-privileged and audited.
- Only authorized maintainers manage Actions secrets and deployment credentials.
- Assign one accountable human per PR.

## Repository ownership

- `aegora-docs` — canonical PRD, architecture, ADRs, and team engineering workflow.
- `aegora-frontend` — UI/application shell, typed API clients, E2E.
- `aegora-backend` — domain policy, API, DB migrations, workers, payment adapters.
- `aegora-contracts` — Solidity/Hardhat, ABI exports, deployments, contract tests.
- `.github` — GitHub defaults and organizational governance only.

## Development / release

Issue -> plan when needed -> isolated worktree -> implement -> verify -> independent diff review -> author inspection -> PR -> CI -> human review -> squash merge -> staging smoke test.

Details: [`aegora-docs/engineering`](https://github.com/bcd-Aegora/aegora-docs/tree/main/engineering).

## ACP/AHP guidance

Editor ACP and AHP are optional development tooling, not mandatory system components. Different engineers may choose their supported IDE and coding agent. An AHP host only becomes appropriate when there is a real need for shared synchronized agent sessions; do not grant it unbounded GitHub access.
