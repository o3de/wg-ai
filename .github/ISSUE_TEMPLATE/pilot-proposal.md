---
name: 'Pilot Proposal'
about: Propose a WG-AI pilot of AI in project operations (review, triage, housekeeping, safety)
title: Proposed WG-AI Pilot =description=
labels: 'pilot, needs-triage'
assignees: ''

---

# WG-AI Pilot Proposal Template

### When using this template, you do not have to fill out every question below. The questions are there for guidance.

Use this template to propose running an AI tool on O3DE repositories as a WG-AI pilot. Every pilot must follow the [pilot guardrails](https://github.com/o3de/wg-ai/blob/main/pilots/readme.md#guardrails). Once accepted, the pilot gets its own document in the [pilots](https://github.com/o3de/wg-ai/tree/main/pilots) folder.

# ----- DELETE EVERYTHING FROM THE TOP TO THE SUMMARY LINE BELOW WHEN USING TEMPLATE ----- #

### Summary:
Single paragraph explanation of the pilot.

### Area:
- [ ] Code review
- [ ] Triage (labels, duplicates)
- [ ] Housekeeping (stale items, unlinked PRs, release notes)
- [ ] Safety (security screening, spam)
- [ ] Other:

### Where will it run?
- SIG(s) and repositories:
- SIG chair opt-in (link to comment or meeting notes):

### Tool
- Tool name and vendor / self-hosted / bring-your-own-AI:
- Bot account or GitHub App that will act:
- Permissions requested (list each one and why it is needed):
- Terms of use: does the tool's license allow contributing its output? (see the [Linux Foundation Generative AI Policy](https://www.linuxfoundation.org/legal/generative-ai))

### Guardrail checklist
- [ ] AI never merges; a human approves and merges every change.
- [ ] AI reviews are advisory and don't count toward required approvals.
- [ ] Opt-in by the SIG; the SIG chair can turn it off at any time. How to turn it off:
- [ ] Bot posts from a clearly labeled account; every action is public.
- [ ] Least privilege: no write access to branches. SIG-Security review (link):
- [ ] CI load and cost reviewed with SIG-Build (link):

### Metrics
Which of the [WG-AI metrics](https://github.com/o3de/wg-ai/blob/main/pilots/readme.md#metrics) will this pilot measure, and how will the baseline be recorded before it starts?

### Cost
Expected monthly cost and who pays (credits, sponsor, bring-your-own-AI).

### Duration and exit
- Start and end dates:
- What result would make the WG recommend adopting it? Dropping it?

### Are there any open questions?
- What are some of the open questions and potential scenarios that should be considered?
