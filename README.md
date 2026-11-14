# The Freelance Developer Constitution

### A human–AI partnership for affordable, independent software creation

> **People should be free to build, understand, own, modify, move, and share their software—regardless of income, credentials, or chosen platform. AI exists to expand human capability, not replace human authority.**

This repository holds the **Open Creator Constitution** and practical guidance for developers, AI coding agents, small businesses, students, and independent creators. It began with one mission: make powerful software development and AI-assisted creation accessible to people who cannot afford expensive development tools, while preserving their freedom to leave a platform and keep what they built.

**Our priorities, in order:** freedom → creation → helping others → personal accomplishment. Financial sustainability matters because it keeps the tools available and improving—not because creators should be locked in.

## Core commitments

1. **Human authority:** AI may propose, design, build, explain, and test, but people retain decision-making, ownership, accountability, and final release approval.
2. **Meaningful free access:** Prefer a real no-cost or self-hosted path for learning, building, inspecting, and exporting. Explain resource costs clearly.
3. **Creator ownership:** Users retain rights to their original work, subject to applicable laws, agreements, and third-party licenses.
4. **Freedom to leave:** Projects should be exportable, documented, and usable outside the original platform. No paid upgrade solely to export user-owned source or data.
5. **True open-source practice:** Clearly license code and disclose which components and providers are not open source. Public source alone is not a software license.
6. **Evidence, not promises:** Clearly separate proposed, implemented, tested, and deployed functionality; never claim verification that did not happen.
7. **Privacy and security:** Protect credentials, separate user and admin powers, isolate creators' data, and require consent for consequential operations.
8. **Provider independence:** Favor replaceable AI integrations, documented formats, and portability over hidden vendor dependencies.
9. **Community accountability:** Document decisions, invite contributions, and review tradeoffs openly without sacrificing creator rights.
10. **Verifiable releases:** Check functionality, security, affordability, ownership, portability, accessibility, and authorized human approval.

## A living, adaptable constitution

This is a **starting point, not a final rulebook**. We invite developers, students, independent creators, and human–AI teams to propose improvements, question assumptions, and create new interpretations. The upstream repository has human review and a documented amendment process; independent editions are meant to remain free to evolve under the terms of an appropriate content license.

Read the [Living Constitution](LIVING_CONSTITUTION.md) for how amendments, disagreement, forks, and AI contributions work, and [Contributing](CONTRIBUTING.md) for how to participate. **The intended right to copy and redistribute adapted text still requires an explicit license**, which has not yet been selected.

**First round of feedback**

What would you change? If a paywall or a tool switch made it hard to keep your work, share what happened and what would have helped. Join the [first feedback thread](https://github.com/brandonbright84-web/the-freelance-developer-Constitution/issues/1).

## Read the constitutional documents

| File | Purpose |
| --- | --- |
| [CONSTITUTION.md](CONSTITUTION.md) | Foundational articles, human–AI partnership pledge, governance, decision principles, and definition of done. |
| [LIVING_CONSTITUTION.md](LIVING_CONSTITUTION.md) | Ongoing evolution, community amendments, independent adaptations, and governance boundaries. |
| [CONTRIBUTING.md](CONTRIBUTING.md) | Practical instructions for proposals, pull requests, reviews, attribution, and AI-assisted contributions. |
| [AGENTS.md](AGENTS.md) | Instructions for AI coding agents and human collaborators before, during, and after changes. |
| [RELEASE_CHECKLIST.md](RELEASE_CHECKLIST.md) | Evidence-based PR/release gates and a Constitution Impact Statement template. |
| [APP_WORKSHOP_FOUNDATION.md](APP_WORKSHOP_FOUNDATION.md) | A proposed translation of these principles into App Workshop architecture and testable milestones. |

## How to adopt it in a development project

1. Read the [full constitution](CONSTITUTION.md) and [Living Constitution](LIVING_CONSTITUTION.md), including adaptation, exception, and amendment guidance.
2. Review the draft with the project's human maintainers and record whether and how it is adopted.
3. Copy `CONSTITUTION.md`, `AGENTS.md`, and `RELEASE_CHECKLIST.md` into the project's repository and link them from its README and pull-request process.
4. Choose and add an explicit open-source `LICENSE` for software you intend to release as open source; review dependencies and contributor rights. This constitution is **not** a substitute for a software license.
5. Add project-specific run, build, test, export/import, and independent-deployment instructions.
6. For material changes, record an impact statement on creator freedom, cost, portability, security, AI provider independence, and human approval.

## Example application: App Workshop

App Workshop is intended to make it easier for creators to build, review, export, import, collaborate on, and deploy applications with human-controlled AI assistance. The [foundation blueprint](APP_WORKSHOP_FOUNDATION.md) proposes separate user/admin roles, secure provider adapters, reviewable code generation, a portable export format, independent hosting, and cost limits.

**Important:** The blueprint is a design direction, **not proof that these capabilities are implemented or tested**. In particular, source export, clean-environment import, and independent deployment must be verified before they are claimed as working features.

These principles can also be adopted by other projects, including QuoteCheck, without requiring the projects to share the same technology stack.

## Human and AI partnership

> **Human creativity establishes the destination. Artificial intelligence expands the possible routes. Evidence determines whether we've arrived.**

**Humans:** Set goals, approve important decisions, review evidence, remain accountable, and protect creator rights.

**AI systems:** Offer ideas and implementations, disclose uncertainty, explain tradeoffs, report tests honestly, respect access boundaries, and seek approval for sensitive or irreversible actions.

**Together:** Build tools that people can afford, understand, trust, own, improve, and take with them.

## Status and licensing

- **Constitution version:** 0.1.1, proposed draft.
- **Adoption/ratification:** Not formally recorded in these documents.
- **Software/content license:** Not selected. **Do not assume that a public repository grants open-source reuse rights.** The maintainers should choose and add an appropriate license before describing the materials themselves as open-source licensed.
- **Contributions:** Suggestions and discussions are welcome; see [CONTRIBUTING.md](CONTRIBUTING.md). Because licensing remains undecided, discuss permissions before submitting substantial copyrighted material.

References: [Open Source Definition](https://opensource.org/osd) · [OSI-approved licenses](https://opensource.org/licenses) · [AGENTS.md convention](https://agents.md/)

---

**Guiding test:** *Nobody should have to remain our customer to remain the owner of what they created.*
