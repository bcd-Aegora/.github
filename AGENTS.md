# AGENTS.md — Aegora `.github` (org policies)

Keep organization-wide GitHub policies and templates here. Do not put product architecture or Solidity sources in this repo.

## Explain after coding

Whenever you finish writing or changing code (or project structure/docs that affect how the system works), end with a short teaching-style recap the user can reuse in interviews or reviews:

1. **What changed** — the behavior or capability change in plain language (not a raw file dump).
2. **Why** — the problem or goal this solves.
3. **How it works** — the important control flow, data flow, or design decision (not a line-by-line dump).
4. **How we know** — for auth, policy, payment, migration, or other high-risk changes: the check, test, or evidence that supports the change. Omit when not relevant.
5. **Key terms** — briefly define anything non-obvious introduced in that change (e.g. ABI, `.gitkeep`, registry). Omit when nothing new was introduced.

Keep it clear and exam-friendly. Prefer concrete examples from the change over generic theory. Do this even for small cleanups when they affect understanding of the project. Skip empty optional sections rather than padding them.
