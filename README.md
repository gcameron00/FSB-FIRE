# FSB FIRE Reference

An unofficial reference site for the Financial Stability Board's **Format for Incident Reporting Exchange (FIRE)** — the international standard for harmonised operational incident reporting by financial institutions.

## What is FIRE?

FIRE defines 87 information items that financial institutions provide to authorities when reporting operational incidents (including cyber incidents). Published by the FSB on 15 April 2025, it is designed to:

- Reduce the reporting burden for internationally active firms by aligning fields across jurisdictions
- Support regulatory data-sharing between authorities
- Provide a structured, machine-readable format (XBRL taxonomy + DPM data dictionary)

Reports are submitted in up to three escalating phases — **Initial**, **Intermediate**, and **Final** — requiring 19, 33, and 48 essential items respectively. Of the 87 total items, 48 are essential by the final report and 39 are optional (at each implementing authority's discretion).

## This site

The official FSB publication is the authoritative source, but navigating 87 fields and 14 annexes across a 100-page PDF has friction. This site provides searchable, hyperlinked documentation of the standard.

**This is an independent reference resource. It is not affiliated with or endorsed by the FSB.**

Hosted on [Cloudflare Pages](https://pages.cloudflare.com).

---

## Site structure

| Path | Status | Description |
|------|--------|-------------|
| `/` | Done | Homepage — FIRE overview, stats, and navigation |
| `/about/` | Done | About FIRE and this site |
| `/reference/` | Done | Reference index — links to all tools |
| `/reference/incident-types/` | Done | Annex C — 5 incident type categories |
| `/reference/discovery-methods/` | Done | Annex D — 18 discovery methods |
| `/reference/severity/` | Done | Annex E — six-level severity scale |
| `/reference/disruption-types/` | Done | Annex F — service disruption type classifications |
| `/reference/resources/` | Done | Annexes H–I — resource types and properties |
| `/reference/impact/` | Done | Annexes J–M — financial, operational, reputational, external impact scales |
| `/reference/cause-types/` | Done | Annex N — two-tier cause taxonomy |
| `/docs/reference/fire-field-reference.html` | Done | Interactive field reference (87 items, filterable) |

---

## Local development

No build tools required. Open any `.html` file directly in a browser, or serve the root with a static file server:

```sh
# Python
python -m http.server 8080

# Node
npx serve .
```

## Deployment

The site deploys automatically to Cloudflare Pages on push to `main`.

---

## Roadmap

### Phase 1 — Foundation
- [x] Interactive field reference (87 items, search + filter by group / status / phase)
- [x] About page — FIRE overview and site purpose
- [x] Homepage — FIRE overview, key stats, group list, and navigation
- [x] Consistent site-wide navigation component
- [ ] Move field reference to a clean URL (`/reference/fields/`)

### Phase 2 — Annex reference pages
- [x] Reference index page (`/reference/`)
- [x] Incident types (Annex C — 5 categories)
- [x] Discovery methods (Annex D — 18 methods)
- [x] Standardised severity scale (Annex E — 6 levels: Nil → Extreme)
- [x] Service disruption types (Annex F — Availability, Integrity, Confidentiality, Trust loss)
- [x] Resource types and properties (Annexes H–I)
- [x] Impact scales (Annexes J–M — financial, operational, reputational, external; each 6 levels)
- [x] Cause taxonomy (Annex N — 6 Level-1 categories, 30+ Level-2 subcategories)

### Phase 3 — Guides
- [ ] Reporting phase guide — what is required at each of the three phases and how requirements escalate
- [ ] Field-by-field guidance — notes on implementing optional fields, unstructured text guidance
- [ ] Cross-jurisdiction notes — where authorities have customised the optional fields

---

## Attribution

Source: Financial Stability Board, *Format for Incident Reporting Exchange (FIRE): Final report*, 15 April 2025. The official document is the authoritative reference for all field definitions and requirements.
