# O3DE AI Contribution Policy

> **Status: DRAFT. Not ratified.** This is the WG-AI starting point, taken from the strawman principles in [o3de/tsc#159](https://github.com/o3de/tsc/issues/159). It is not project policy until the TSC ratifies it.

## Principles

1. **A human is responsible.** The person who signs off a contribution under the DCO owns it, whatever tools produced it.
2. **Understand what you submit.** Contributors must be able to explain and defend every change in their PR.
3. **Disclose meaningful AI assistance** in the PR description. Disclosure isn't a reason to reject a PR. *(Undecided: see the disclosure questions below.)*
4. **Keep PRs reviewable.** One issue per PR. Large mechanical changes are allowed when labeled as mechanical.
5. **Respect licensing.** Follow the [Linux Foundation Generative AI Policy](https://www.linuxfoundation.org/legal/generative-ai): the tool's terms must allow contributing its output, and any third-party material it reproduces must be properly licensed and attributed.
6. **AI assists reviewers but never replaces them.** AI reviews are advisory, and a human approves and merges.

## Open questions

Questions marked **(v1)** should be answered before policy v1 goes to the TSC on 2027/01/23. The rest can follow in later versions.

### Legal (for Linux Foundation counsel)

- **(v1) Signing the DCO for AI output.** The DCO certifies the contribution was "created in whole or in part by me" or is based on suitably licensed prior work. Can a contributor honestly sign it for AI-generated code? Uncertainty about exactly this is why some projects ban AI contributions outright, so the rest of this policy depends on the answer.
- **Copyright in AI output.** In the US, the Copyright Office's position is that material without human authorship can't be copyrighted. If a contribution is mostly AI-generated, what is being licensed under Apache-2.0 OR MIT, and does that matter to the project?
- **Assets, not just code.** Can AI-generated textures, models, audio, shaders, levels or docs images be contributed to O3DE's asset and sample repos? Image and audio models carry different training-data risks from code models.
- **Disclosure and legal exposure.** Should contributors disclose AI assistance at all? A record of which tool or model produced a change is searchable. If a model maker is later sued over its training data, could that record expose the project or its contributors? Leaving disclosure out doesn't change what is in the code, and the DCO sign-off already makes the human responsible for it. Options:
  - Name the tool or model (commit trailer or PR note).
  - Generic "AI-assisted" with no tool named.
  - No disclosure; the DCO sign-off carries the responsibility.

  **Ask Linux Foundation counsel:** does recording which AI tool or model was used increase the project's or contributors' exposure, compared with saying nothing or saying only "AI-assisted"?

### Disclosure

- **Tool-added trailers.** Some AI tools add attribution trailers such as `Co-authored-by: Claude` to commits by default. 34 of the 1,068 commits on o3de `development` since 2025 already carry one. Whatever the disclosure answer, the policy must say whether these trailers are expected, allowed or should be removed.
- If disclosure is kept: what counts as "meaningful" AI assistance, and what form does it take (a PR template checkbox, a trailer, free text)?

### Confidentiality: what never goes into an AI tool

- **(v1) Code under NDA.** Restricted platform code and console SDK material must not be pasted into hosted AI tools. Likely a rule rather than a question; the WG needs to agree the wording.
- **Porting from other engines.** Asking an AI to port a feature from Unreal or another proprietary engine imports code O3DE can't license. Is porting from license-compatible engines, such as Godot (MIT), acceptable with attribution?
- **Embargoed and private data.** May maintainers put unpublished vulnerability details, user crash dumps or private Discord messages into AI tools?

### Who can act

- **(v1) Autonomous agents.** May a bot or agent open PRs or issues, or answer review comments, with no human driving it? Must a human open every PR?
- **AI-written issues and security reports.** Other projects, curl among them, have been flooded with AI-generated vulnerability reports that weren't real. How does O3DE handle invented bug and security reports? With SIG-Security.
- **Commit identity.** Agents committing under their own identity or a made-up one. Confirm the DCO check accepts only a real person's sign-off.

### Contributions and review

- What size limit, if any, applies to a PR, and how is "mechanical" defined and labeled?
- Should an issue be required for every PR?
- **Reviewers using AI.** May reviewers use AI tools, and must they say so? Who is responsible when a reviewer approves on AI findings they didn't check?
- **Good first issues.** If AI solves them, newcomers lose their way in. Should good first issues be kept for people learning the codebase?

### Enforcement

- **(v1) Enforcing without AI detectors.** Detectors are unreliable, so the policy shouldn't depend on guessing whether something was AI-written. What may a reviewer ask for instead, for example "explain this change in your own words"?
- What may a reviewer do with a PR that doesn't meet the policy: request changes, close it, or label it and move on?
- **Repeat offenders.** What happens to someone who keeps sending low-quality AI PRs, who decides, and how does that tie to the Code of Conduct?
- **AI-written code already merged.** 34 commits already carry AI trailers. Likely answer: no audit. The policy should say so explicitly.

### Scope and upkeep

- **(v1) Which repos the policy covers.** o3de, o3de-extras, the docs, SIG repos, and 3p-package-source, where supply-chain risk is highest.
- How does the policy avoid disadvantaging contributors who don't use AI tools or can't access them?
- **Review schedule and ownership.** AI tools change every few months. How often is the policy reviewed, and who owns it after the WG ends: SIG-AI or the TSC?
