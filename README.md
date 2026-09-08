# JKDD Leads — Public Website Preview V1

Product key: `jkdd_leads`

## Status

- Environment: Development / Preview
- Hosting target: GitHub Pages (zero-cost static hosting)
- Production application: UNTOUCHED
- Backend: NOT CONNECTED in this preview
- Secrets: NONE

## Governance

This package follows the JKDD Leads product boundary and JKDD TECH Foundation rules:

1. REUSE BEFORE BUILD.
2. ONE SOURCE OF TRUTH.
3. ONE DOMAIN OWNER.
4. FOUNDATION BEFORE LOCAL IMPLEMENTATION.
5. NO PARALLEL ARCHITECTURE.
6. ONE LEAD → ONE CANONICAL RECORD → MULTIPLE PRODUCT VIEWS.

### Existing capability found

JKDD TECH Foundation owns shared identity/session/company/RBAC/RLS/audit/settings capabilities. The public marketing preview does not duplicate them.

### Canonical owner

JKDD Leads owns Lead, Lead Source, Lead Lifecycle Event, Lead Score, Lead Qualification, Lead Assignment, Lead Routing, Lead Status History, Acquisition Attribution, Deduplication and Enrichment.

### Reuse method

Static marketing website only. Any future authenticated area or real intake must consume Foundation contracts and the canonical JKDD Leads intake service.

### Actual gap

A public zero-cost marketing presence and GitHub Pages-ready frontend were missing.

### New code required

YES — static public website assets only.

## Preview behavior

The Early Access form is intentionally local-only. It stores preview entries in the visitor browser `localStorage` and sends nothing to a server. This avoids inventing a parallel lead backend before the canonical intake endpoint is ready.

## Files

- `index.html` — landing page
- `styles.css` — responsive visual system
- `script.js` — PT/EN language toggle, navigation, reveal effects and local-only preview form
- `assets/favicon.svg` — preview product mark
- `manifest.webmanifest` — basic install metadata
- `.nojekyll` — GitHub Pages static mode
- `404.html` — simple Pages fallback

## Deployment gate

Repository: `joukinneto/jkdd-leads-site`

Workflow:

1. Work on `feat/public-site-preview-v1`.
2. Review through pull request.
3. Merge only with publication authorization.
4. Enable GitHub Pages from `main` / root.

Do not place API keys, Supabase service-role keys, private tokens or other secrets in this repository.

## Future integration backlog

- Replace preview Early Access storage with canonical JKDD Leads intake endpoint.
- Add Foundation-based authenticated login only when the public product portal is formally scoped.
- Add official product social links when accounts are created.
- Add canonical product icon/brand assets after Preview approval.
- Add analytics only through an approved privacy/governance decision; avoid paid tooling by default.
