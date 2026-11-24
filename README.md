# 2026 Global DTC & K-Beauty Lookalike Domain, Email Auth & AI-Citation Benchmark Dataset (N = 48)

Published by **Sentinel Threat Lab (AboutUsAgency, Inc.)** · Captured **November 23, 2026** · License: **CC BY 4.0**

- **Interactive Report & Full Methodology:** https://sentineldefense.io/research/2026-dtc-lookalike-study
- **Reproduce Any Row Live (Free, No Login):**
  - 16-Variant Lookalike DNS & RDAP Radar: https://sentineldefense.io/phish
  - 0–100 AI-Citation Readiness Auditor: https://sentineldefense.io/ai-reputation
  - Zero-Upload Creator DNS/CDN/RDAP & DMCA § 512 Dissector: https://sentineldefense.io/piracy
  - 42-Broker Global Privacy Matrix (CCPA / GDPR / APPI / PDPL): https://sentineldefense.io/privacy
  - 10-Minute Zero-Webhook Partner Program: https://sentineldefense.io/partners

## Summary Findings (Unfiltered — Zero Cherry-Picking, Includes All 0-Hit Rows)

| Metric | Value | Notes |
| :--- | :--- | :--- |
| Storefronts audited | **48** | US DTC, US Beauty, Global DTC, K-Beauty, K-Fashion |
| Total resolving lookalikes | **238 domains** | Mean **4.96** resolving variants per storefront across **15–16** candidates (top: Allbirds `13/16`, Alo Yoga `11/16`, Ridge `11/16`, COSRX `10/16`, Medicube US `10/16`) |
| Missing SPF or DMARC TXT | **10 / 48 (21%)** | Includes apex stores missing `_dmarc` (e.g., COSRX, SOME BY MI) and regional subdomains lacking host SPF |
| AI-Citation Readiness < 70/100 | **35 / 48 (73%)** | Common causes: WAF HTTP 403/429 bot walls, missing root `Organization` + `sameAs` JSON-LD, missing `/llms.txt` |

## Files Included

- [`dtc-lookalike-ai-benchmark-2026-11-23.csv`](./dtc-lookalike-ai-benchmark-2026-11-23.csv) — Flat CSV for Pandas, DuckDB, Excel, or SQL analysis.
- [`dtc-lookalike-ai-benchmark-2026-11-23.json`](./dtc-lookalike-ai-benchmark-2026-11-23.json) — Structured JSON with aggregate metadata and all 48 rows.

## Important Methodological Caveats

1. **Defensive vs. Third-Party Registrations:** Resolving lookalike DNS counts include defensive domains registered by the brand itself, parked domains, and third-party registrations. Brands must cross-check active permutations against their internal registrar inventory before filing abuse notices.
2. **Subdomain SPF/DMARC Inheritance:** Regional storefronts (such as `us.laneige.com` or `en.abib.com`) may inherit apex DMARC while lacking host-level SPF TXT records.
3. **100% Public Passive Telemetry:** Every measurement was gathered via unauthenticated public DNS (`A`/`NS`/`TXT`), public RDAP lookups, and standard HTTP requests.
4. **Compliance Boundary:** AboutUsAgency, Inc. is a software company, not a law firm, and does not provide legal advice or guarantee takedown outcomes.
