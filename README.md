# Pearl (pearl-dental)

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
