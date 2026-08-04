# Pearl (pearl-dental)

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

Pearl is a dental AI computer-vision company (West Hollywood, CA; founded 2019; CEO Ophir Tanz). Its FDA-cleared products deliver AI at the point of care by embedding into third-party dental imaging and practice management software rather than through a public, self-serve developer API:

- **Second Opinion** — real-time pathology and restorative detection on 2D and 3D (CBCT) dental radiographs. Detects up to 18 findings per image (incipient/progressed caries, bone loss with millimeter and ratio measurements, calculus, periapical radiolucencies, defective margins, widened PDL, impactions) plus existing restorations (crowns, fillings, bridges, root canals, implants), returned as labeled bounding boxes overlaid on the image. 95%+ accuracy; 90%+ of images processed in under one minute.
- **Practice Intelligence** — clinical and operational analytics pairing Pearl's diagnostic AI with full practice-management-system data (clinical quality, financial performance, appointment compliance, case acceptance, per-provider production) across one location or hundreds.
- **Precheck** — AI insurance claim review / claims automation.

## Access model — partner / OEM gated (important)

**Pearl does not publish a public, self-serve developer API, SDK, or OpenAPI reference.** There is no developer portal, no API key signup, and no published API reference. Pearl's AI is provisioned through imaging/PMS partners and direct sales to practices and DSOs:

- **40+ native integrations** including DEXIS, Carestream, Planmeca Romexis, Dentsply Sirona Sidexis, Apteryx XVWeb, MiPACS, Open Dental, Dentrix, Eaglesoft, Carestack, Oryx, Curve, Denticon, and Software of Excellence EXACT.
- **Authorized vendor in the Henry Schein One API Exchange** (Dentrix / Dentrix Ascend).
- **Custom integrations** for any system that "exposes a public API or accessible data layer" — i.e. Pearl typically *consumes* a partner's API rather than publishing its own — delivered in ~40 business days.
- Provisioned customers are managed through the **Pearl Management Portal** (management.hellopearl.com), with a standalone web app (secondopinion.hellopearl.com) and a Help Center (help.hellopearl.com).

Because there is no published Pearl API reference, the API surfaces documented here are **modeled** from Pearl's public product and integration descriptions and are tagged **Modeled** / **Partner Gated**. No OpenAPI, endpoint paths, schemas, or auth were fabricated, and no `openapi/`, `rate-limits/`, `finops/`, or `collections/` artifacts were created.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/pearl-dental/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/pearl-dental/refs/heads/main/apis.yml)

## Tags

- AI
- Dental
- Computer Vision
- Radiology
- Medical Imaging
- Pathology Detection
- Healthcare
- Partner Gated

## Timestamps

- **Created:** 2026-07-05
- **Modified:** 2026-07-05

## APIs (modeled, partner-gated)

### Pearl Second Opinion Image Analysis API

Partner/OEM-gated cloud AI surface behind Second Opinion. Integrated imaging software submits a radiograph (bitewing, periapical, panoramic, or CBCT) and receives detections and measurements as labeled bounding boxes and metadata. No public developer reference; endpoints are modeled from product descriptions.

- **Human URL:** [https://hellopearl.com/products/second-opinion](https://hellopearl.com/products/second-opinion)

### Pearl Practice Intelligence Analytics API

Analytics pairing diagnostic AI with full PMS data (clinical quality, financials, appointment compliance, case acceptance, per-provider production). Integrates by consuming a PMS that exposes a public API or accessible data layer. No public Pearl developer API; surface is modeled.

- **Human URL:** [https://hellopearl.com/products/practice-intelligence](https://hellopearl.com/products/practice-intelligence)

### Pearl PMS Integration Exchange API

Partner/vendor enablement layer through which Pearl is provisioned inside imaging/PMS systems, including as an authorized vendor in the Henry Schein One API Exchange, and managed via the Pearl Management Portal. Not a public developer API; endpoints are modeled.

- **Human URL:** [https://www.hellopearl.com/press-release/pearl-joins-henry-schein-one-api-exchange-as-an-authorized-integration-vendor](https://www.hellopearl.com/press-release/pearl-joins-henry-schein-one-api-exchange-as-an-authorized-integration-vendor)

## Plans and pricing

Contact-sales / partner-gated. Pearl publishes no price list, self-serve signup, or metered developer-API pricing. See [plans/pearl-dental-plans-pricing.yml](plans/pearl-dental-plans-pricing.yml) for the commercial model and clearly-attributed third-party observed price points (e.g. Second Opinion observed at ~$299/month per location; setup fees observed at ~$5,000–$20,000; enterprise/DSO negotiated). All figures are third-party observations, not an official Pearl rate card.

## Common Properties

- [LinkedIn](https://www.linkedin.com/company/hellopearl)
- [Website](https://hellopearl.com)
- [Documentation](https://help.hellopearl.com)
- [Integrations](https://www.hellopearl.com/native-integration)
- [Portal](https://management.hellopearl.com/)
- [Plans](plans/pearl-dental-plans-pricing.yml)
- [Blog](https://hellopearl.com/blog)

## WebSocket review

Pearl does **not** expose a documented public WebSocket API — and does not expose a public developer API of any kind. See [review.yml](review.yml).

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
