<div align="center">

# Stefano Seggio

### Founder, Delta Registry — Pay-Per-Event Regulatory & Compliance Data Infrastructure

**28 live Apify Actors · 38 open-source repositories · Buenos Aires, Argentina**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/stefanoseggio-deltaregistry)
[![Apify Store](https://img.shields.io/badge/Apify%20Store-View%20Fleet-FF9012?style=for-the-badge&logo=apify&logoColor=white)](https://apify.com/stefano_seggio)
[![Enterprise Licensing](https://img.shields.io/badge/Enterprise-Licensing-1a1a2e?style=for-the-badge)](https://www.linkedin.com/in/stefanoseggio-deltaregistry)

</div>

---

## Executive Summary

Delta Registry is a pay-per-event (PPE) data infrastructure operation: 28 hosted Apify Actors that turn government registries, regulatory feeds, and compliance-adjacent public data sources into structured, delta-aware event streams. Every actor in the fleet shares the same design discipline — a dual-fingerprint (or hash-based) delta engine that tracks state across runs, a documented Pay-Per-Event pricing model billed only for genuinely new or changed records, zero-infrastructure hosting on Apify's platform, and honest, disclosed limitations rather than smoothed-over marketing copy. The fleet spans six practice areas: government procurement and grants, regulatory enforcement and litigation, patent and trademark monitoring, sanctions and compliance screening, AI/content infrastructure, and financial markets/sovereign debt.

This profile is the entry point to the whole fleet. Every listing below links to either a real, open-source integration repository (README, architecture diagram, Node.js/Python SDK snippets) or, for actors not yet mirrored to their own repository, directly to the live Apify Store listing.

## Featured — 2026-09 Fleet Expansion

Five new Actors shipped this cycle, each targeting a compliance-data niche with no existing structured feed:

| Actor | What it does | Pricing (from) | Links |
|---|---|---|---|
| **AI Crawler & Content-Signal Permission Delta Monitor** | Delta-monitors `robots.txt` AI-crawler permissions (GPTBot, ClaudeBot, 16 others), Cloudflare Content-Signal headers, and `llms.txt` for changes | $0.006/event | [Repo](https://github.com/stefanoseggio/ai-crawler-content-signal-permission-monitor) · [Store](https://apify.com/stefano_seggio/ai-crawler-content-signal-permission-monitor) |
| **Regione Lombardia Open Grants & Tenders Registry Delta Monitor** | Turns Regione Lombardia's Socrata `bandi` registry into a NEW_LISTING/STATUS_CHANGE/UPDATED delta feed | $0.008/event | [Repo](https://github.com/stefanoseggio/regione-lombardia-grants-registry-monitor) · [Store](https://apify.com/stefano_seggio/regione-lombardia-grants-registry-monitor) |
| **SEC Enforcement & Litigation Release Delta Feed** | Structures SEC.gov's own litigation-release and administrative-proceeding RSS feeds into EDGAR CIK-linked records | $0.02/event | [Repo](https://github.com/stefanoseggio/sec-enforcement-litigation-delta-feed) · [Store](https://apify.com/stefano_seggio/sec-enforcement-litigation-delta-feed) |
| **KIPRIS Patent & Trademark Status-Change Monitor** | Bring-your-own-key delta monitoring for Korean patent/utility-model filings on KIPRIS Plus | $0.008/event | [Repo](https://github.com/stefanoseggio/kipris-patent-trademark-status-monitor) · [Store](https://apify.com/stefano_seggio/kipris-patent-trademark-status-monitor) |
| **Aozora Bunko New Public-Domain Text Delta Feed** | Live delta feed of newly digitized, confirmed-public-domain Japanese literature for NLP/digital-humanities pipelines | $0.01/event | [Repo](https://github.com/stefanoseggio/aozora-bunko-public-domain-text-feed) · [Store](https://apify.com/stefano_seggio/aozora-bunko-public-domain-text-feed) |

> All five are now live on the Apify Store. KIPRIS Patent & Trademark Status-Change Monitor's earlier platform-side publish error cleared and it went public on 2026-09-17.

## Featured — 2026-09-17 Institutional Fleet Expansion

Four new Actors shipped this cycle, extending the fleet into public procurement (EU-wide), UK statutory compliance, sovereign-debt markets, and Gulf corporate registries:

| Actor | What it does | Pricing (from) | Links |
|---|---|---|---|
| **EU TED Procurement Delta Monitor** | Delta-tracks EU public procurement notices — new tenders, contract awards, status changes — across all 27 member states via TED's official public Search API | $0.01/event | [Repo](https://github.com/stefanoseggio/eu-ted-procurement-delta-monitor) · [Store](https://apify.com/stefano_seggio/eu-ted-procurement-delta-monitor) |
| **UK Modern Slavery Statement Registry Delta Monitor** | Delta-tracks the official UK Modern Slavery Statement Registry — 34,000+ organisations — for new statements, compliance-status changes, and missing mandatory disclosures | $0.01/event | [Repo](https://github.com/stefanoseggio/uk-modern-slavery-statement-registry-monitor) · [Store](https://apify.com/stefano_seggio/uk-modern-slavery-statement-registry-monitor) |
| **Emerging-Market Sovereign Debt Auction Monitor** | Delta-tracks Brazil's National Treasury domestic bond auction results (LTN, LFT, NTN-B, NTN-F) for new auctions and marginal-rate/coverage-ratio anomalies | $0.01/event | [Repo](https://github.com/stefanoseggio/emerging-market-sovereign-debt-auction-monitor) · [Store](https://apify.com/stefano_seggio/emerging-market-sovereign-debt-auction-monitor) |
| **UAE Corporate Registry Monitor** | Delta-tracks UAE corporate registrations and license-status changes across Dubai mainland (Dubai Pulse), ADGM, and DIFC public registers | $0.01/event | [Repo](https://github.com/stefanoseggio/uae-corporate-registry-monitor) · [Store](https://apify.com/stefano_seggio/uae-corporate-registry-monitor) |

> All four are live on the Apify Store as of 2026-09-17. Honest status note: ADGM and DIFC (two of the UAE actor's three data sources) are currently affected by live, ongoing outages on those registries' own servers (a NullPointerException on ADGM's side, an HTTP 500 on DIFC's) — confirmed independently, unrelated to this actor's code, and being monitored via a standalone health probe shipped in that actor's own repository.

## The Full Fleet

### Government Procurement & Grants

| Actor | Coverage | Repository |
|---|---|---|
| Florida Tenders Monitor | MyFloridaMarketPlace — ITB/RFP/ITN solicitations and awards | [Repo](https://github.com/stefanoseggio/florida-tenders-monitor) |
| Buenos Aires Province Tenders Monitor | PBAC portal — upcoming, recent, and awarded processes | [Repo](https://github.com/stefanoseggio/pba-tenders-monitor) |
| Australia GrantConnect Monitor | grants.gov.au — recipient, ABN, agency, value, program | [Repo](https://github.com/stefanoseggio/australia-grantconnect-monitor) |
| Regione Lombardia Grants & Tenders Monitor | dati.lombardia.it Socrata bandi registry | [Repo](https://github.com/stefanoseggio/regione-lombardia-grants-registry-monitor) |
| Mendoza Compras Monitor | Province of Mendoza, Argentina — licitaciones/contrataciones | [Repo](https://github.com/stefanoseggio/mendoza-compras-monitor) |
| Cordoba Compras Monitor | Province of Cordoba, Argentina — public tenders | [Repo](https://github.com/stefanoseggio/cordoba-compras-monitor) |
| Entre Rios Compras Monitor | Province of Entre Rios, Argentina — public tenders | [Repo](https://github.com/stefanoseggio/entrerios-compras-monitor) |
| Salta Compras Monitor | Province of Salta, Argentina — public tenders | [Repo](https://github.com/stefanoseggio/salta-compras-monitor) |
| Tucuman Compras Monitor | Province of Tucuman, Argentina — public tenders | [Repo](https://github.com/stefanoseggio/tucuman-compras-monitor) |
| Santa Fe Compras Monitor | Province of Santa Fe, Argentina — public tenders | [Repo](https://github.com/stefanoseggio/santafe-compras-monitor) |
| EU TED Procurement Delta Monitor | TED (Tenders Electronic Daily) — new tenders, contract awards, status changes across all 27 EU member states | [Repo](https://github.com/stefanoseggio/eu-ted-procurement-delta-monitor) |

### Financial Markets & Sovereign Debt

| Actor | Coverage | Repository |
|---|---|---|
| Emerging-Market Sovereign Debt Auction Monitor | Brazil National Treasury bond auctions (LTN, LFT, NTN-B, NTN-F) — new auctions, rate/coverage anomalies | [Repo](https://github.com/stefanoseggio/emerging-market-sovereign-debt-auction-monitor) |

### Regulatory Enforcement, Litigation & Compliance

| Actor | Coverage | Repository |
|---|---|---|
| SEC Enforcement & Litigation Release Delta Feed | SEC.gov litigation releases + administrative proceedings | [Repo](https://github.com/stefanoseggio/sec-enforcement-litigation-delta-feed) |
| UK HSE Enforcement Monitor | HSE convictions, fines, enforcement notices | [Repo](https://github.com/stefanoseggio/uk-hse-enforcement-monitor) |
| Maritime Sanctions Monitor | OFAC SDN vessel list cross-referenced against the UN Consolidated List | [Repo](https://github.com/stefanoseggio/actor-19-maritime-sanctions-monitor) |
| MDB Procurement Monitor | World Bank Procurement Notices + Other Sanctions | [Repo](https://github.com/stefanoseggio/actor-20-mdb-procurement-monitor) |
| Patent & IP Enforcement Monitor | USPTO PTAB + EPO OPS, with a dedicated TERMINATED signal | [Repo](https://github.com/stefanoseggio/actor-21-patent-ip-enforcement-monitor) |
| Drug Safety & Recalls Monitor | FDA openFDA recalls + EMA DHPC safety alerts | [Repo](https://github.com/stefanoseggio/actor-22-drug-safety-recalls-monitor) |
| Diario Oficial Chile Monitor | Chile's official gazette — laws, decrees, resolutions | [Repo](https://github.com/stefanoseggio/diario-oficial-cl-monitor) |
| Singapore ACRA Registry Monitor | Singapore corporate registry — new listings/status changes | [Repo](https://github.com/stefanoseggio/singapore-acra-registry-monitor) |
| UK Modern Slavery Statement Registry Delta Monitor | UK Modern Slavery Statement Registry — new statements, compliance-status changes, missing disclosures | [Repo](https://github.com/stefanoseggio/uk-modern-slavery-statement-registry-monitor) |
| UAE Corporate Registry Monitor | Dubai mainland (Dubai Pulse), ADGM, and DIFC — new registrations, license-status changes | [Repo](https://github.com/stefanoseggio/uae-corporate-registry-monitor) |

### Patent, Trademark & Clinical Data

| Actor | Coverage | Repository |
|---|---|---|
| KIPRIS Patent & Trademark Status-Change Monitor | Korean patent/utility-model filings (BYOK) | [Repo](https://github.com/stefanoseggio/kipris-patent-trademark-status-monitor) |
| Clinical Trials Delta Engine | ClinicalTrials.gov API v2 + FDA Orange Book — trial status and patent/exclusivity delta feed | [Repo](https://github.com/stefanoseggio/actor-24-clinical-trials-delta-engine) · [Apify Store](https://apify.com/stefano_seggio/actor-24-clinical-trials-delta-engine) · [Sample stub](https://github.com/stefanoseggio/delta-registry-clinicaltrials-full-stub) |

### AI Infrastructure, Content & Lead Generation

| Actor | Coverage | Repository |
|---|---|---|
| AI Crawler & Content-Signal Permission Delta Monitor | robots.txt AI-crawler permissions, Content-Signal, llms.txt | [Repo](https://github.com/stefanoseggio/ai-crawler-content-signal-permission-monitor) |
| Aozora Bunko Public-Domain Text Delta Feed | Newly digitized Japanese public-domain literature | [Repo](https://github.com/stefanoseggio/aozora-bunko-public-domain-text-feed) |
| Page Metadata Extractor | SEO/RAG metadata — title, OG tags, canonical URL, H1, word count | [Repo](https://github.com/stefanoseggio/primer-actor) |
| B2B Lead Magnet | Compliant lead discovery (seed list / OSM Overpass) + enrichment waterfall | [Repo](https://github.com/stefanoseggio/actor-18-b2b-lead-magnet) |

### Supporting Infrastructure

| Repository | Purpose |
|---|---|
| [delta-registry-website](https://github.com/stefanoseggio/delta-registry-website) | Marketing site — architecture, pricing, delta-engine internals (Next.js 14, Vercel) |
| [awesome-regulatory-monitors](https://github.com/stefanoseggio/awesome-regulatory-monitors) | Unified Python/Node.js SDKs and monitoring suite across the fleet |
| `delta-registry-*-stub` (7 repos) | Free, one-off sample pullers demonstrating each production Actor's real data shape before you commit to a paid run |

## Design Principles Across the Fleet

- **Pay only for signal.** Every Actor bills on a Pay-Per-Event model — a baseline/no-diff record is always free; you're charged only when something genuinely new or changed is delivered.
- **Delta-aware by default.** Cross-run state (SHA-256 or content-hash fingerprints, persisted in a named Key-Value Store) means a scheduled run reports only what moved since the last check, never a full re-dump.
- **Zero infrastructure.** No server, cron host, proxy pool, or session-cookie logic to maintain — Apify's platform runs the schedule, the retries, and the persisted state.
- **Disclosed limitations, not hidden ones.** Every Actor's README states what it cannot do (fuzzy name matching, source refresh cadence, PDF text-layer failures) as plainly as what it can.
- **BYOK where the underlying data source is itself a paid product** (e.g. KIPRIS Plus) — so operator margin never rides on marking up someone else's license.

## GitHub Activity

<div align="center">

![GitHub Streak](https://github-readme-streak-stats.herokuapp.com/?user=stefanoseggio&theme=tokyonight&hide_border=true)

</div>

<!-- Note: the github-readme-stats.vercel.app badges (contribution stats, top languages) are omitted — the shared public Vercel deployment is currently returning DEPLOYMENT_PAUSED for all users, verified 2026-09-18. Re-add once that instance is back, or switch to a self-hosted deployment. -->

## Stack

![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=node.js&logoColor=white)
![Apify](https://img.shields.io/badge/Apify-FF9012?style=flat-square&logo=apify&logoColor=white)
![Crawlee](https://img.shields.io/badge/Crawlee-1EA7FD?style=flat-square)
![Cheerio](https://img.shields.io/badge/Cheerio-E88C1F?style=flat-square)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)

## Work With Delta Registry

- **Run any Actor today** — browse the full catalog at [apify.com/stefano_seggio](https://apify.com/stefano_seggio); every listing is pay-per-event with no subscription.
- **Enterprise licensing, custom monitors, or a new jurisdiction added to an existing fleet** — reach out directly on [LinkedIn](https://www.linkedin.com/in/stefanoseggio-deltaregistry).
- **Integrating via API** — every repository above ships real Node.js and Python `apify-client` examples under `examples/`; no SDK to install beyond the official Apify client.

---

<div align="center">
<sub>Delta Registry is built and operated by Stefano Seggio, Buenos Aires, Argentina. Connect on <a href="https://www.linkedin.com/in/stefanoseggio-deltaregistry">LinkedIn</a>.</sub>
</div>
