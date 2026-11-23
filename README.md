# O3DE AI Working Group (WG-AI)

The AI Working Group is a short-lived, cross-SIG group chartered by the O3DE Technical Steering Committee. It defines how O3DE uses AI as a project and how contributors may use it, then hands that work to a permanent SIG-AI.

- **Formed:** 2026-11-17, by TSC resolution on [o3de/tsc#159](https://github.com/o3de/tsc/issues/159)
- **Lifespan:** 6 months from formation (to about 2027-05-17). The TSC can extend it by vote.
- **Charter:** [governance/WG AI Charter.md](governance/WG%20AI%20Charter.md)
- **Meetings:** weekly, Mondays at 10:00 Pacific / 19:00 CET, in the [WG-AI Discord channel](https://discord.com/channels/805939474655346758/1052633353695793172). See [meetings](meetings/readme.md).

## Why this group exists

The Linux Foundation has a [Generative AI Policy](https://www.linuxfoundation.org/legal/generative-ai), but O3DE has no written position on AI. Contributors already send AI-generated pull requests, and maintainers already use AI to review them, with no shared rules. The TSC raised the topic at most meetings from August 2026 on, agreed it needs a policy "in writing", and agreed it is too large to settle in a regular TSC agenda slot.

AI cuts across every SIG. A policy owned by any one SIG wouldn't bind the others, so the TSC formed a working group, which is quicker to stand up than a SIG and has a fixed purpose and lifespan.

## What WG-AI does

1. **AI contribution policy.** Draft a one-page policy, small and clear, for TSC ratification. See [policy](policy/readme.md).
2. **AI in project operations.** Pilot AI code review, issue and PR triage, SIG labeling, housekeeping and safety screening, and measure whether they help. See [pilots](pilots/readme.md).
3. **Tooling and resources.** Compare candidate tools, find free or discounted AI credits, and recommend how to track cost and usage.
4. **Making O3DE readable by AI tools.** Recommend agent instruction files (for example `AGENTS.md`), an `llms.txt` for the docs site, and ways to surface knowledge that lives only in Discord. With SIG-Docs-Community.
5. **SIG-AI charter.** Write the scope, membership rules and ownership boundaries for a permanent SIG-AI and present it to the TSC.
6. **Defending the repositories against attacks.** With SIG-Security, write a strategy against attacks that AI makes cheaper, such as backdoored or spam PRs and supply-chain attacks, and against prompt injection aimed at the project's own AI tools.

AI features in the engine itself (ML gems, in-editor assistants, AI-driven tools) are exploratory only: the WG lists existing efforts and recommends who should own them. The WG doesn't build engine features.

## What WG-AI does not do

- Require any AI tool for contributors or maintainers.
- Change review or merge permissions directly. The WG recommends; the TSC and the SIGs decide.
- Override a SIG's own review rules. Each SIG keeps final say in its area.
- Interpret law. Licensing questions go to Linux Foundation counsel.

## Deliverables

| Month | Target | Deliverable | Status |
|---|---|---|---|
| 1 | 2026-12 | WG formed: leadership confirmed, repo created, weekly meetings running | In progress |
| 2 | 2027-01 | **AI contribution policy v1** presented to the TSC for ratification | Not started |
| 2–4 | 2027-01 to 2027-03 | Pilots: AI review and triage labeling in SIG-Platform repos, then volunteer SIGs, with baseline metrics recorded before each starts | Not started |
| 5 | 2027-04 | Pilot report: what to adopt project-wide, what to drop, and what it costs (including bring-your-own-AI) | Not started |
| 6 | 2027-05 | **SIG-AI charter** presented to the TSC. The WG closes when the TSC accepts it or decides not to form SIG-AI | Not started |

## Leadership

**Leadership is a commitment to do work. It is not authority.**

The people on the leadership team have volunteered to be responsible for the working group's products and deadlines. They have committed to:

- attend every meeting,
- run the meetings,
- see that the deliverables are written and delivered on time,
- merge pull requests to this repository, since they hold merge permission on it.

That's all. Being on the leadership team gives no special authority over the WG's decisions. **Anyone at all interested can participate, and their voice carries the same weight as a lead's.** When the WG votes, leads vote the same as everyone else, one voice each. The leads decide among themselves who is responsible for what.

The TSC adopted the WG on 2026-11-17 and seated all nominees without a vote, since there were fewer nominees than seats.

| Discord | GitHub | Responsible for |
|---|---|---|
| colinb[APMG] | [byrcolin](https://github.com/byrcolin) | *TBD* |
| ladyfia \| Iris | [LadyManaa](https://github.com/LadyManaa) | *TBD* |
| JT[SCB_Network] | [JT-SCB-GameDesign](https://github.com/JT-SCB-GameDesign) | *TBD* |
| Shauna [Genome Studios] | [ShaunaGordon](https://github.com/ShaunaGordon) | *TBD* |
| Astin(Chogan) | [Astin-A](https://github.com/Astin-A) | *TBD* |

More volunteers can join the leadership team at any later TSC meeting. No more than two leads should be from the same employer.

## SIG liaisons

Each SIG can name one liaison so policy drafts reflect how that SIG actually reviews and triages. Use the [nomination template](.github/ISSUE_TEMPLATE/Leadership_Liaison_Nomination.md).

| SIG | Liaison | Involvement |
|---|---|---|
| SIG-Platform | *TBD* | Hosts the first pilots |
| SIG-Security | *TBD* | Reviews tool permissions and the security screening pilot; co-writes the repository defense strategy |
| SIG-Build | *TBD* | Reviews CI cost and load |
| SIG-Docs-Community | *TBD* | Docs and community knowledge readable by AI tools |
| Other SIGs | *TBD* | Opt in to pilots; keep final say over their own review rules |

## How to engage

- **Discord.** Join the [WG-AI channel](https://discord.com/channels/805939474655346758/1052633353695793172) on the O3DE Discord.
- **Meetings.** Anyone can attend. Agendas are issues in this repo labeled `mtg-agenda`; add a topic by commenting on the next one. See [meetings](meetings/readme.md).
- **Proposals.** Open an issue using one of the [templates](.github/ISSUE_TEMPLATE): a policy or process suggestion, or a pilot proposal.
- **Watch this repo** for drafts, notes and pilot reports. Pull requests to this repo are the WG's paper trail.

## How we decide

- **Open membership.** Anyone in the community can join and take part.
- **Lazy consensus** by default. If there's an objection, a majority of the people attending a WG meeting decides. Leads count the same as anyone else.
- **TSC ratification.** Policy documents take effect only after the TSC ratifies them.
- **Transparency.** Meeting notes, drafts and pilot reports are public in this repo.

## Repository layout

| Path | Contents |
|---|---|
| [governance/](governance) | WG charter; the SIG-AI charter draft when it exists |
| [policy/](policy/readme.md) | AI contribution policy drafts |
| [pilots/](pilots/readme.md) | Pilot guardrails, metrics, and one document per pilot |
| [meetings/](meetings/readme.md) | Agendas, notes, media and resources |
| [rfcs/](rfcs/readme.md) | Accepted RFCs |

## Licensing

This repository and all contributions to it are licensed under the [Creative Commons Attribution 4.0 International License](http://creativecommons.org/licenses/by/4.0/). By contributing to this repository, whether via commit, pull request, issue, comment, or in any other fashion, **you agree that your contributions fall under the same license.**
