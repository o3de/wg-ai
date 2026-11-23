# WG-AI Pilots

The WG evaluates AI in project operations by running small, opt-in pilots on O3DE repositories, starting with SIG-Platform's. Each pilot gets one document in this folder: what it tries, where it runs, the tool and its permissions, the baseline metrics, and the results.

Propose a pilot with the **Pilot Proposal** issue template.

## Pilot areas

| Area | What it tries |
|---|---|
| Code review | AI review comments on PRs: advisory only or counting toward approvals, and which findings block a merge |
| Triage | Applying `sig/*` labels, triage labels and duplicate links to new issues and PRs |
| Housekeeping | Finding stale issues and PRs, flagging PRs with no linked issue, drafting release notes |
| Safety | Screening PRs for security problems and moderating spam before a human reviews them |

## Guardrails

Every pilot follows these rules, from the [charter](../governance/WG%20AI%20Charter.md):

1. **AI never merges.** A human approves and merges every change.
2. **AI reviews are advisory** and don't count toward required approvals, unless the TSC votes otherwise after seeing pilot results.
3. **Pilots are opt-in per SIG.** SIG-Platform goes first. Any SIG chair can turn a pilot off in their area at any time.
4. **AI actions are visible.** Bots post from clearly labeled accounts, and every action they take on GitHub is public.
5. **Least privilege.** Pilot tools get only the permissions they need, such as labels and comments, with no write access to branches. SIG-Security reviews tool permissions first.
6. **No CI cost surprises.** Coordinate with SIG-Build before anything adds load to automated review (AR) builds.

## Metrics

Record a baseline before each pilot starts, then measure the same things during it.

- Time from a PR opening to its first review.
- Share of new issues and PRs triaged and labeled within 7 days.
- Label accuracy: the share of AI-applied labels a human had to correct.
- Review usefulness: the share of AI review findings that maintainers acted on.
- Maintainer and contributor feedback, from a short survey at the end of each pilot.
- Cost per month.

## Pilots

| Pilot | SIG / repos | Status | Document |
|---|---|---|---|
| *None yet* | | | |
