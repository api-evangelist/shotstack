# Shotstack (shotstack)

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

Shotstack is a cloud video-editing platform that turns a JSON timeline into a rendered video, image, or audio file. The Edit API renders programmatically from a JSON edit specification and templates, the Ingest API uploads and transforms source footage, the Serve API hosts and delivers generated assets, and the Create API generates AI assets such as text-to-speech, text-to-image, and image-to-video.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/shotstack/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/shotstack/refs/heads/main/apis.yml)

## Tags

- Video
- Video Editing
- Media
- Rendering
- Generative AI

## Timestamps

- **Created:** 2026-06-20
- **Modified:** 2026-06-20

## APIs

### Shotstack Edit (Render) API

Queue a video, image, or audio render from a JSON edit specification (timeline, tracks, clips, output) and poll render status by ID. Supports AI generative assets (text-to-speech, text-to-image, image-to-video) embedded in the timeline.

- **Human URL:** [https://shotstack.io/docs/api/](https://shotstack.io/docs/api/)
- **Base URL:** `https://api.shotstack.io/edit/v1`

#### Tags

- Video Editing
- Rendering
- Timeline

#### Properties

- [Documentation](https://shotstack.io/docs/guide/architecture/apis/)
- [API Reference](https://shotstack.io/docs/api/)
- [OpenAPI](openapi/shotstack-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/shotstack.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/shotstack.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Shotstack Templates API

Save, list, retrieve, update, and delete reusable edit templates, then render them with merge-field variable substitution for data-driven, automated video generation at scale.

- **Human URL:** [https://shotstack.io/docs/api/](https://shotstack.io/docs/api/)
- **Base URL:** `https://api.shotstack.io/edit/v1`

#### Tags

- Templates
- Merge Fields
- Automation

#### Properties

- [Documentation](https://shotstack.io/docs/guide/templates/templates/)
- [API Reference](https://shotstack.io/docs/api/)
- [OpenAPI](openapi/shotstack-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/shotstack.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/shotstack.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Shotstack Ingest API

Upload, store, and transform source footage, images, audio, and fonts from a URL or direct upload, with optional renditions and transcription, ready for use by the Edit API.

- **Human URL:** [https://shotstack.io/docs/api/](https://shotstack.io/docs/api/)
- **Base URL:** `https://api.shotstack.io/ingest/v1`

#### Tags

- Ingest
- Assets
- Transcoding

#### Properties

- [Documentation](https://shotstack.io/docs/guide/ingesting-footage/ingest-api/)
- [API Reference](https://shotstack.io/docs/api/)
- [OpenAPI](openapi/shotstack-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/shotstack.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/shotstack.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Shotstack Serve API

Inspect, manage, and delete the hosting of assets generated by the Edit and Ingest APIs, retrieve CDN URLs by asset or render ID, and transfer files to external destinations.

- **Human URL:** [https://shotstack.io/docs/api/](https://shotstack.io/docs/api/)
- **Base URL:** `https://api.shotstack.io/serve/v1`

#### Tags

- Serving
- Hosting
- CDN

#### Properties

- [Documentation](https://shotstack.io/docs/guide/serving-assets/serve-api/)
- [API Reference](https://shotstack.io/docs/api/)
- [OpenAPI](openapi/shotstack-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/shotstack.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/shotstack.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Shotstack Create (AI Assets) API

Generate AI assets - text-to-speech, text-to-image, image-to-video, and text generation - through built-in (Shotstack) and third-party (ElevenLabs, Stability AI) providers, returning hosted assets for use in renders.

- **Human URL:** [https://shotstack.io/docs/api/](https://shotstack.io/docs/api/)
- **Base URL:** `https://api.shotstack.io/create/v1`

#### Tags

- Generative AI
- Text to Speech
- Text to Image

#### Properties

- [Documentation](https://shotstack.io/product/create-api/)
- [API Reference](https://shotstack.io/docs/api/)
- [OpenAPI](openapi/shotstack-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/shotstack.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/shotstack.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [GitHub Organization](https://github.com/shotstack)
- [LinkedIn](https://www.linkedin.com/company/shotstack)
- [Website](https://shotstack.io)
- [Documentation](https://shotstack.io/docs/)
- [Plans](plans/shotstack-plans-pricing.yml)
- [Rate Limits](rate-limits/shotstack-rate-limits.yml)
- [Fin Ops](finops/shotstack-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
