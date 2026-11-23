# WG-AI Charter

This charter records the AI Working Group as proposed in [o3de/tsc#159](https://github.com/o3de/tsc/issues/159) and adopted by the TSC on 2026-11-17. The TSC charter allows it to create ["sub-committees or working groups to focus on cross-project technical issues and requirements"](https://github.com/o3de/tsc/blob/ac76c289ad18e29b5d24e70db785a64ed91e1b9b/README.md?plain=1#L97-L109).

Team information is in the [README](../README.md).

# Overview of WG

Defines how O3DE uses AI as a project, and how contributors may use it, then hands that work to a permanent SIG-AI.

- **Formed:** 2026-11-17
- **Started:** 2026/11/23, the first WG meeting. All timeline dates in this charter count from this day.
- **Lifespan:** 6 months (2027/05/23), ending with a formal proposal for SIG-AI and its charter. The TSC can extend the WG by vote if the work isn't finished.

# Goals

1. Draft the project's official AI policy for TSC ratification.
2. Pilot AI in project operations, such as code review, issue and PR triage, and SIG labeling, and measure whether it helps.
3. Write the charter for a permanent SIG-AI to own this area once the WG ends.

# Scope

## In scope

**1. AI contribution policy.** One page, small and clear, ratified by the TSC. It covers:

* Accountability. The human who signs the DCO owns the contribution, whatever tools produced it.
* Whether and how contributors disclose AI assistance.
* PR size and focus rules, with an exception for mechanical changes.
* Whether contributors must understand and be able to explain their change.
* Tool licensing and third-party content, aligned with the [Linux Foundation Generative AI Policy](https://www.linuxfoundation.org/legal/generative-ai).
* What reviewers may do with a PR that doesn't meet the policy.

**2. AI in project operations.** Evaluate and pilot:

* **Code review.** AI review on PRs. Decide whether it is advisory only or counts toward the required approvals, and which findings block a merge, for example only criticals and blockers.
* **Triage.** Applying SIG labels (`sig/*`), triage labels and duplicate links to new issues and PRs, so SIG chairs spend less time on routine sorting.
* **Housekeeping.** Finding stale issues and PRs, flagging PRs with no linked issue, and drafting release notes.
* **Safety.** Screening PRs for security problems and moderating spam before a human reviews them.

**3. Tooling and resources.**

* Compare candidate tools: hosted review bots, the GitHub-native options, and self-hosted or bring-your-own-AI setups.
* Find free or discounted AI credits through the Linux Foundation, foundation members and vendor open-source programs.
* Recommend how to track cost and usage.

**4. Making O3DE readable by AI tools.** Recommend agent instruction files for the main repos (for example `AGENTS.md`), an `llms.txt` for the docs site, and ways to make knowledge that now lives only in Discord findable. Work with SIG-Docs-Community on this.

**5. A SIG-AI charter.** Write the scope, membership rules and ownership boundaries for the permanent SIG, and present it to the TSC.

## Exploratory, with a recommendation only

* **AI features in the engine itself**, such as ML gems, in-editor assistants and AI-driven tools. The WG will list existing efforts and recommend whether SIG-AI should own them, share them with existing SIGs, or leave them alone. The WG won't build engine features.

## Out of scope

* Requiring any AI tool for contributors or maintainers.
* Changing review or merge permissions directly. The WG recommends; the TSC and the SIGs decide.
* Overriding a SIG's own review rules. Each SIG keeps final say in its area.
* Legal interpretation. Licensing questions go to Linux Foundation counsel.

## Cross-cutting processes

The WG works through the existing SIGs and doesn't replace any of them.

| SIG | Involvement |
|---|---|
| SIG-Platform | Volunteers to host the first pilots. |
| SIG-Security | Reviews tool permissions and the security screening pilot. |
| SIG-Build | Reviews CI cost and load. |
| SIG-Docs-Community | Works on making docs and community knowledge readable by AI tools. |
| All SIGs | Can name a liaison to speak for their SIG. Opt in to pilots. Keep final say over their own review rules. |

# Guardrails for pilots

Any pilot the WG runs on O3DE repositories follows these rules:

1. **AI never merges.** A human approves and merges every change.
2. **AI reviews are advisory** and don't count toward required approvals, unless the TSC votes otherwise after seeing pilot results.
3. **Pilots are opt-in per SIG.** SIG-Platform goes first. Any SIG chair can turn a pilot off in their area at any time.
4. **AI actions are visible.** Bots post from clearly labeled accounts, and every action they take on GitHub is public.
5. **Least privilege.** Pilot tools get only the permissions they need, such as labels and comments, with no write access to branches. SIG-Security reviews tool permissions first where it has the resources.
6. **No CI cost surprises.** Coordinate with SIG-Build before anything adds load to automated review (AR) builds.

# Deliverables and timeline

| Month | Deliverable |
|---|---|
| 1 (2026/12/23) | WG formed: leadership team confirmed, repo created, weekly WG meetings on Discord. |
| 2 (2027/01/23) | **AI contribution policy v1** presented to the TSC for ratification. |
| 2–4 (2026/12/23 to 2027/03/23) | Pilots: AI review and triage labeling in SIG-Platform repos, then in volunteer SIGs. Baseline metrics recorded before each pilot starts. |
| 5 (2027/04/23) | Pilot report with recommendations: what to adopt project-wide, what to drop, and what it costs, including bring-your-own-AI. |
| 6 (2027/05/23) | **SIG-AI charter** presented to the TSC. The WG closes when the TSC accepts the charter or decides not to form SIG-AI. |

# How pilots are measured

* Time from a PR opening to its first review.
* Share of new issues and PRs triaged and labeled within 7 days.
* Label accuracy: the share of AI-applied labels a human had to correct.
* Review usefulness: the share of AI review findings that maintainers acted on.
* Maintainer and contributor feedback, from a short survey at the end of each pilot.
* Cost per month.

# WG links and lists

- Repository: [o3de/wg-ai](https://github.com/o3de/wg-ai)
- GitHub team: `@o3de/wg-ai`, maintained by the leadership team
- Discord: [WG-AI channel](https://discord.com/channels/805939474655346758/1052633353695793172)
- Issues / PRs: [issues](https://github.com/o3de/wg-ai/issues), [pull requests](https://github.com/o3de/wg-ai/pulls)
- Meeting agendas & notes: [meetings](../meetings/readme.md)
- Formation: [o3de/tsc#159](https://github.com/o3de/tsc/issues/159)

# Roles and Organization Management

## Leadership team

**Leadership is a commitment to do work. It is not authority.**

The leadership team are people who have volunteered to be responsible for the WG's products and deadlines. Leads commit to:

* attend every WG meeting,
* run the meetings,
* see that the deliverables are written and delivered on time, including reporting to the TSC and keeping the paper trail,
* merge pull requests to this repository, since they hold merge permission on it.

That is the whole of the role. Being a lead gives no special authority over the WG's decisions. Leads take part and vote the same as anyone else, with one voice each. The leads decide among themselves who is responsible for what, and record it in the [README](../README.md).

Leadership should come from more than one SIG and more than one organization, and no more than two leads should be from the same employer. The TSC confirms leads at a TSC meeting. More volunteers can join the leadership team the same way at any later meeting.

## Members

Membership is open. Anyone in the community who is at all interested can join and take part, and their voice carries the same weight as a lead's.

## SIG liaisons

Each SIG can name one liaison, so policy drafts reflect how each SIG actually reviews and triages.

## Decisions

* Lazy consensus by default. If there's an objection, a majority of the people attending a WG meeting decides. Leads count the same as anyone else.
* Policy documents take effect only after TSC ratification.
* Meeting notes and drafts are public in this repo. Pull requests to the repo are the paper trail.

# Resources

* GitHub repository `o3de/wg-ai` for notes, drafts and pilot reports.
* GitHub team `@o3de/wg-ai`, maintained by the leadership team.
* A WG-AI Discord channel.
* Approval to install pilot tools (GitHub Apps or bot accounts) on repositories whose SIGs opt in, after SIG-Security review.
* Help from Linux Foundation and O3DF staff in asking for open-source AI credits.

# Path to SIG-AI

The WG will recommend forming SIG-AI if, by month 6 (2027/05/23):

* The TSC has ratified the AI contribution policy and it needs ongoing ownership.
* At least one pilot has shown value worth keeping as permanent project infrastructure.
* Enough regular contributors exist to staff a SIG's chair, co-chair and maintainer roles.

If those conditions aren't met, the WG will recommend where its outputs should live instead. For example, the policy could live with the TSC and the tools with SIG-Operations.

# Note on process

O3DE has no written procedure for creating a working group. The TSC charter allows WGs, but the steps have so far existed only in meeting discussion. This WG followed the steps the TSC described: a written charter, a presentation at a TSC meeting, feedback, and ratification. The TSC may adopt this charter's structure as the template for future WG proposals.
