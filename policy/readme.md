# O3DE AI Contribution Policy

This folder holds drafts of the project's AI contribution policy. The WG's target is **v1 presented to the TSC in month 2 (2027/01/23)**. A draft takes effect only after the TSC ratifies it.

- [AI Contribution Policy (draft).md](AI%20Contribution%20Policy%20(draft).md): the working draft, seeded from the strawman principles in [o3de/tsc#159](https://github.com/o3de/tsc/issues/159).
- [AGENTS.md](AGENTS.md): proposed instructions for AI coding agents, to sit at the root of [o3de/o3de](https://github.com/o3de/o3de). Its ground rules follow the policy draft, so it lands upstream after the policy is ratified.
- [CLAUDE.md](CLAUDE.md): a one-line import of `AGENTS.md` for Claude Code, which reads only `CLAUDE.md` in older versions and ignores `AGENTS.md` whenever a `CLAUDE.md` exists. Goes upstream with `AGENTS.md`.

## What the policy must cover

From the [charter](../governance/WG%20AI%20Charter.md):

- Accountability. The human who signs the DCO owns the contribution, whatever tools produced it.
- Whether and how contributors disclose AI assistance.
- PR size and focus rules, with an exception for mechanical changes.
- Whether contributors must understand and be able to explain their change.
- Tool licensing and third-party content, aligned with the [Linux Foundation Generative AI Policy](https://www.linuxfoundation.org/legal/generative-ai).
- What reviewers may do with a PR that doesn't meet the policy.

## Concerns raised so far

Raised on [o3de/tsc#159](https://github.com/o3de/tsc/issues/159) and in TSC meetings. The policy should answer each.

- Code becoming hard to maintain for contributors who don't use AI.
- Contributors who can't get AI tools, because of cost, token access or geofencing.
- Giving the wider community, beyond those on Discord and GitHub daily, time to read and comment before ratification.
- Keeping the focus on quality for users, not on making AI contribution easier.

## How to propose a change

Open a pull request against the draft, or an issue using the **Policy/Process Suggestion** template. Discuss it at a WG meeting. When the WG reaches consensus, a lead brings the draft to the TSC.
