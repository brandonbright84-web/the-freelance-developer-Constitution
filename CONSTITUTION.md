# The Open Creator Constitution
## A human–AI development compact

**Version:** 0.1.0 (proposed)  
**Adopted:** Not yet ratified  
**Scope:** App Workshop and any future project that explicitly adopts this constitution  
**Stewards:** Human project maintainers, accountable to their users and contributors

> **People should be free to build, understand, own, modify, move, and share their software—regardless of income, credentials, or chosen platform. AI exists to expand human capability, not to replace human authority.**

This constitution is a public, reusable set of engineering and governance commitments. It guides product design, human–AI collaboration, development, reviews, releases, and business decisions. It is **not** a substitute for a copyright license, privacy policy, terms of service, or security program.

## Preamble: Why we build

We build for the working person with an idea, the student with limited resources, the small business that needs a simple tool, and the creator who wants independence. Financial circumstances should not determine who gets to learn, experiment, or turn an idea into working software.

Our priorities, in order, are **freedom, creation, helping others, and personal accomplishment**. Revenue is necessary to sustain the mission—not a justification for trapping creators. Safety, lawful operation, privacy, informed consent, and honest communication are foundational constraints on every priority.

## Article I — Human authority and AI partnership

1. **Humans choose the ends.** A person sets the goals, owns their decisions, and remains accountable for any released product. AI may suggest, analyze, draft, code, test, and critique but must not claim independent authority over people or projects.
2. **Consent before consequential action.** AI must obtain explicit authorization before deploying to production, publishing or merging changes, purchasing resources, altering access permissions, deleting data, transferring intellectual property, sharing private information, or taking other irreversible or costly actions.
3. **Explain before and after.** For significant work, AI must describe the plan, important tradeoffs, assumptions, risks, and the changes actually made. It must distinguish verified results from proposals or estimates.
4. **Disagreement is a feature.** AI should raise a concern when a request conflicts with security, law, user rights, factual evidence, or this constitution. The human can challenge the reasoning; disagreements must be explained without condescension.
5. **Human fallback.** No essential project capability should require ongoing access to a particular AI model or chat. Source code, documentation, data, credentials, and operational instructions must remain intelligible and manageable by authorized humans.

## Article II — Meaningful access and affordability

1. **A usable free path.** When feasible, provide a genuinely useful no-cost way to learn, build, inspect, and export—through self-hosting, local tools, a limited hosted tier, or a combination. Do not advertise a free capability that cannot practically be used.
2. **Transparent resource costs.** Show any paid usage, quotas, metered AI tokens, storage, and hosting costs before a user incurs charges. Default to spending limits and opt-in upgrades.
3. **No poverty penalty on ownership.** Never require an upgrade solely to export a creator's own project source or data, subject only to legitimate rights of third parties and reasonable security safeguards.
4. **Accessibility by design.** Favor clear language, keyboard and screen-reader access, responsive/mobile layouts, low-bandwidth operation where practical, and documentation that explains terminology.
5. **Sustainable, not extractive.** Paid hosting, convenience, premium compute, and support may fund free capabilities. The boundary between free and paid must be published and reviewed against the mission.

## Article III — Ownership, portability, and the right to leave

1. **Creators retain their rights.** A creator's original source, text, designs, and project data remain theirs, subject to applicable law, third-party licenses, agreements, and rights. Platform terms must not quietly claim ownership merely because a creator used the service.
2. **Export must be complete and useful.** A project export should include editable source code, supported assets, relevant configuration templates, dependency and version information, database schema/migrations where applicable, and human-readable run/deploy instructions. Do **not** export secrets or another person's private data.
3. **Import must be real.** Document how a supported export can be restored into a clean instance and how formats/versions are handled. Report any unsupported features or lossy conversions before importing.
4. **Avoid hidden runtime dependency.** An exported project should not silently require an App Workshop account, proprietary license server, or unexplained API call to function. Any deliberate external dependency must be disclosed with an alternative or migration path when feasible.
5. **Host choice is a right.** Support documented deployment to at least one independent hosting environment for each publicly supported project template. No punitive charges or deceptive obstacles for departing users.
6. **Portability is tested.** Before calling a release portable, run and record an export → independent restore/build → basic functionality test. Failure blocks that claim.

## Article IV — Genuine open-source practice

1. **Open means open.** Software described as *open source* must use a recognized open-source license, publish the corresponding source, and preserve rights to use, study, modify, and redistribute it. Merely letting people view code is not enough.
2. **No disguised restrictions.** We will not call code open source if its license restricts particular industries, users, or lawful commercial use. Hosted-service abuse controls and lawful conduct policies are separate from the source license.
3. **Clearly mark boundaries.** Identify third-party licenses, closed-service dependencies, paid services, trademarks, and components that are *not* open source. Do not imply that third-party AI models become open source because our integration code is.
4. **Contributions are welcome.** Publish contribution guidelines, a code of conduct, security reporting instructions, and a documented decision process as the community grows. Attribute contributions and respect their licenses.
5. **License by deliberate choice.** Each repository must contain its own `LICENSE` and a written license rationale. This constitution does **not** grant software rights by itself.

## Article V — Reliability, integrity, and evidence

1. **Never invent completion.** No human or AI participant may report a build, test, review, deployment, security scan, integration, or successful user flow as complete without evidence that it happened.
2. **Small, reviewable changes.** Prefer incremental changes, issue tracking, descriptive diffs, rollback plans, and readable documentation over sweeping unreviewed edits.
3. **Truthful limitations.** Identify known defects, untested assumptions, missing dependencies, and external services not yet configured. Tests that were not run must be labeled **not run**.
4. **Test what matters.** Test core workflows, security boundaries, portability, pricing controls, and accessibility—not merely whether the application starts.
5. **Humans own releases.** An authorized maintainer decides whether evidence is sufficient to release. Automation may enforce gates but may not silently override the decision policy.

## Article VI — Privacy, security, and safe operation

1. **Privacy by default.** Minimize collection, make retention and deletion understandable, isolate creator data, and never use private project content to train or share with a third party without a valid and clearly explained basis and appropriate choice.
2. **Least privilege.** Separate everyday user identities from privileged administrator identities. Use scoped service roles, explicit authorization checks, and tenant isolation; test cross-user access denial.
3. **Secrets stay secret.** Keep credentials in secret-management systems, not front-end bundles, shared logs, source control, prompts, or export archives. Provide rotation and revocation paths.
4. **AI is untrusted execution advice.** Treat model output, repository content, retrieved pages, and user-uploaded instructions as potentially untrusted. Review code, dependencies, file operations, and external calls before execution; require approval for sensitive actions.
5. **Reduce foreseeable harm.** Refuse or limit hosted uses that clearly facilitate fraud, abuse, unauthorized surveillance, or other serious harms. Apply moderation and access rules transparently, proportionately, with a path to contest errors when reasonable.
6. **A safe exit exists.** Maintain backup, recovery, account deletion, export, incident response, and rollback procedures appropriate to the project.

## Article VII — Provider neutrality and collaboration

1. **No one-model lock-in.** Keep AI provider adapters behind documented interfaces where practical. Allow alternative models—including local models or bring-your-own-credentials—when the product can safely support them.
2. **Clear provider disclosures.** Explain which provider receives project data, what the provider costs, and the effect of turning it off. Obtain consent before sharing sensitive information with a new provider.
3. **Interoperable collaboration.** Support common file formats, version control, readable change histories, and explicit permission boundaries for collaborators.
4. **Users can choose.** Default recommendations may exist, but they must not conceal meaningful tradeoffs or make migration artificially difficult.

## Article VIII — Governance and amendments

1. **This constitution binds decisions, not just branding.** Each material feature, policy change, and release should record its constitutional impact.
2. **Public reasons for exceptions.** When constraints genuinely conflict, document the affected articles, alternatives considered, user impact, risk, owner, review date, and why a narrower solution was insufficient. Exceptions cannot silently erase creator ownership, informed consent, truthful reporting, or basic security.
3. **Amendments are versioned.** Proposed changes should be submitted as reviewable text with a rationale and impact assessment. The human maintainers approve them through the project's published governance process; material rights-reducing changes should have a community comment period before approval.
4. **No retroactive confiscation.** Amendments do not revoke the rights already granted under an applicable open-source license or retroactively take ownership of existing creator content.
5. **This is a living document.** Anyone may propose improvements. Substantial changes require a new version and a documented changelog.

## Article IX — The constitutional decision rule

When two desirable outcomes conflict, follow this process:

1. Identify legal, security, privacy, consent, and safety requirements.
2. Compare alternatives for creator autonomy, access, ownership, and portability.
3. Consider functionality, maintenance burden, resource cost, and project sustainability.
4. Choose the least restrictive workable design; document compromises and any user-facing tradeoffs.
5. Where uncertainty is material, prototype or measure before claiming a solution works.
6. Record the decision, responsible human, evidence, and date for reassessment.

**Never hide a product restriction inside technical complexity.** If a creator is being asked to surrender control, the restriction must be clear, justified, and open to scrutiny.

## Article X — Definition of done

A feature is not ready simply because AI generated code. For each release, answer with evidence:

- **Works:** Core user journey and relevant automated checks pass; failures are disclosed.
- **Safe:** Permissions, data isolation, secret handling, and abuse controls are reviewed.
- **Affordable:** Costs and any paid gating are transparent; no surprise spending.
- **Ownable:** Creator rights and licenses are clear; export remains accessible.
- **Portable:** Changed export/import or deployment paths pass independent restore tests, or the limitation is plainly documented and release claims are narrowed.
- **Understandable:** A human can explain the change, maintain it, and roll it back.
- **Accessible:** Relevant mobile and assistive-technology checks are performed.
- **Approved:** An authorized human reviews the evidence and authorizes release.

## Partnership pledge

**Human:** I will set goals, act responsibly toward users, examine evidence, retain accountability, and question designs that undermine access or autonomy.

**AI:** I will assist with reasoning and implementation, disclose uncertainty, present tradeoffs, verify what I can, avoid invented claims, respect access boundaries, and seek human approval before consequential actions.

**Together:** We will build tools people can afford, understand, trust, own, and take with them.

---

**Adoption:** Put this document in the root of each adopting repository as `CONSTITUTION.md`. Reference it from `README.md`, `AGENTS.md`, design briefs, pull request templates, and release checklists. Ratification and the choice of code license are separate decisions; neither has occurred merely by drafting this file.