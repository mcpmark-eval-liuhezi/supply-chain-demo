# Facilitator Notes — Supply-Chain Security Workshop

Short agenda for the live demo session.

## Session Agenda

1. **Why supply-chain security matters** (5 min)
   - Open-source dependencies as an attack surface; the cost of unpatched critical CVEs.
2. **Where advisories live** (5 min)
   - GitHub Security Advisories (GHSA), the global advisory database, and Dependabot alerts.
3. **Walk through a real critical advisory** (10 min)
   - GHSA-673q-mjm6-r5xr — Next.js unauthenticated RCE in `use cache` functions returning typed arrays (`next`, npm, patched in 16.4.1).
   - See `docs/advisory-example.md` (in the demo pull request) for the summarized details.
4. **The demo repo itself** (10 min)
   - How the advisory was researched, documented on a branch, and turned into a pull request.
   - Show the PR, the review workflow, and keeping a PR branch up to date with `main`.
5. **Takeaways & next steps** (5 min)
   - Enable Dependabot alerts/security updates, pin versions, review what the base branch changes mean for an in-flight PR.

## Facilitator Tips

- Keep the terminal/GitHub UI on screen for the PR walkthrough.
- Emphasize: severity ratings, affected version ranges, and "first patched version" are what drive the actual fix work.
