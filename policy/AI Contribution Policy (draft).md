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

- **Disclosure and legal exposure.** Should contributors disclose AI assistance at all? A record of which tool or model produced a change is searchable. If a model maker is later sued over its training data, could that record expose the project or its contributors? Leaving disclosure out doesn't change what is in the code, and the DCO sign-off already makes the human responsible for it. Options:
  - Name the tool or model (commit trailer or PR note).
  - Generic "AI-assisted" with no tool named.
  - No disclosure; the DCO sign-off carries the responsibility.

  **Ask Linux Foundation counsel:** does recording which AI tool or model was used increase the project's or contributors' exposure, compared with saying nothing or saying only "AI-assisted"?
- **Tool-added trailers.** Some AI tools add attribution trailers such as `Co-authored-by: Claude` to commits by default. 34 of the 1,068 commits on o3de `development` since 2025 already carry one. Whatever the disclosure answer, the policy must say whether these trailers are expected, allowed or should be removed.
- If disclosure is kept: what counts as "meaningful" AI assistance, and what form does it take (a PR template checkbox, a trailer, free text)?
- What size limit, if any, applies to a PR, and how is "mechanical" defined and labeled?
- What may a reviewer do with a PR that doesn't meet the policy: request changes, close it, or label it and move on?
- Should an issue be required for every PR?
- How does the policy avoid disadvantaging contributors who don't use AI tools or can't access them?
