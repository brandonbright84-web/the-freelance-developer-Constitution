# App Workshop: constitution-to-architecture blueprint

**Status:** Proposed design direction, not a claim that any feature currently exists or passes tests.

The constitution requires an architecture that supports creators who are cost-conscious, unfamiliar with deployment, and unwilling to surrender project control.

## Architectural boundaries

| Area | Initial principle | Evidence required before launch |
| --- | --- | --- |
| Identity | Separate ordinary and privileged administrator identities; scope creator memberships per project | Role and unauthorized-access tests |
| Data | Creator/project data isolated by authorization policy and server-side checks | Cross-tenant denial tests |
| AI providers | Swappable adapter interface; BYO credential or local provider where supported | Same sample generation flow across two adapters or documented limitations |
| Secrets | Provider credentials stored server-side in secret storage, never included in exported files | Repository/client-bundle and log inspection |
| Build pipeline | AI creates a draft change set, human inspects diff, isolated tests run, then human approves | Prompt → files → review → test → save trace |
| Export | Download source, assets, dependency manifest, database migrations, and deployment instructions where applicable | Restore project on a clean machine independent of App Workshop |
| Import | Versioned project manifest, validation, conflict and missing-feature report | Reimport a supported exported project without losing documented fields |
| Hosting | Local or user-selected deployment target; hosted option is a convenience | Deploy template on independent platform |
| Cost | Metered hosted AI usage with preview, quotas, caps, and no mandatory paid export | Test zero-budget and capped-budget paths |
| Collaboration | Creator-controlled permissions, transparent revision history, revocable invitations | Permission and revocation tests |

## Suggested implementation sequence

### Milestone 1 — Establish trust boundaries

Document creator, member, ordinary account, administrator, and service roles. Verify authentication and cross-project isolation with real tests. Keep privileged secrets off the client.

**Accept when:** role tests pass, a member cannot read another creator's private project, and no privileged key appears in a client bundle.

### Milestone 2 — Make ownership tangible

Define a versioned portable project manifest and build `export` plus clean-instance `import`. Ensure exports never contain secrets or other creators' data.

**Accept when:** a sample project round-trips and can be built from an exported copy without an App Workshop account.

### Milestone 3 — Add controlled AI building

Implement provider-neutral generation adapters and a review screen. Separate *draft generated* from *tests passed* and *production deployed*. Require explicit approval for sensitive or costly operations.

**Accept when:** a sample prompt creates reviewable files, failures are reported accurately, the user can reject changes, and no unapproved production deployment occurs.

### Milestone 4 — Ship affordable hosted convenience

Add predictable quotas and budget caps, a low-resource starter path, accessible onboarding, and an optional managed deployment experience.

**Accept when:** a zero-budget user can create and export a usable sample project; a paid user sees the price before accepting a charge; and exported projects can leave the platform.

## First architecture decision records (ADRs)

Create separate ADRs to decide: software license (e.g. Apache-2.0 vs a copyleft option); export manifest schema/versioning; provider adapter contract; hosting/runtime boundaries; pricing and cost caps; creator-owned content terms; and governance/ratification. Treat these as decisions to make, not as established facts.