# Alyce

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Alyce is an AI-powered corporate gifting platform that enables B2B sales, marketing, and customer success teams to send hyper-personalized gifts at scale. The platform uses AI to research recipient personal interests and recommends relevant gifts, driving higher engagement and acceptance rates compared to generic gifting approaches.

Alyce was acquired by Sendoso in February 2024 and operated as Alyce by Sendoso, combining two leading intelligent gifting platforms.

## Status: retired (verified 2026-08-13)

**The standalone Alyce product surface is decommissioned.** Probed on 2026-08-13:

| Host | Result |
|---|---|
| `alyce.com`, `www`, `app`, `api`, `docs`, `developer`, `dashboard`, `dashboard-sandbox`, `recipient` | no A/AAAA record at 1.1.1.1, 8.8.8.8 or 9.9.9.9 |
| `help.alyce.com` (documentation) | Cloudflare error 525 — origin down since at least 2025-09-02 |
| `status.alyce.com` | HTTP 200 → `alyce.statuspage.io/inactive`, "Page Inactive" |
| `github.com/alycecom` | HTTP 200, 0 public repositories |

The Internet Archive last records `https://www.alyce.com/` returning 200 on 2025-10-08,
a 301 on 2025-10-09, and a 404 by 2026-01-02. The domain is still registered (expiry
2028-12-14) and still carries Google Workspace MX records, so mail resolves, but the
web product does not. No API, no reachable documentation, and no machine-readable
contract of any kind is available. Full evidence and timeline:
[`lifecycle/alyce-lifecycle.yml`](lifecycle/alyce-lifecycle.yml).

## API (historical)

Alyce provided a REST API at `https://app.alyce.com/api` — a host that no longer
resolves — for programmatic integration with the gifting platform. The API supported:

- Sending personalized gift invitations
- Tracking gift status (sent, accepted, declined, exchanged, donated)
- Managing gift budgets and marketplace configuration
- Triggering gift sends from CRM workflows
- Webhooks for real-time gift event notifications

## Integrations

Alyce integrates natively with:

- **CRM**: Salesforce, HubSpot
- **Marketing Automation**: Marketo, Eloqua
- **Sales Engagement**: Outreach, Salesloft
- **ABM Platforms**: 6sense, Demandbase, RollWorks

## Links

- **Website**: https://www.alyce.com/ — *NXDOMAIN as of 2026-08-13*
- **Documentation**: https://help.alyce.com/collection/357-integrations — *HTTP 525*
- **Blog**: https://www.alyce.com/blog/ — *NXDOMAIN*
- **Status**: https://status.alyce.com/ — *inactive*
- **GitHub**: https://github.com/alycecom — *live, 0 public repos*
- **LinkedIn**: https://www.linkedin.com/company/alyce-co — *live*
- **X**: https://x.com/alycegifts — *live*
- **Acquirer**: https://www.sendoso.com/ — *live*

## APIs.json

This repository contains an [APIs.json](apis.yml) profile cataloging the Alyce API and associated resources including plans, rate limits, and FinOps data.
