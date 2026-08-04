# Studio Ghibli (studio-ghibli)

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

Studio Ghibli API — a community-built, unofficial, fan-made, MIT-licensed REST API that catalogs the people, places, and things found in the worlds of Studio Ghibli. Five resource collections (films, people, locations, species, vehicles) cross-link via canonical URLs. No authentication, no metering, no paid tier. Source: github.com/janaipakos/ghibliapi (archived 2022-12-02); canonical instance now at ghibliapi.vercel.app.

**APIs.json:** [https://ghibliapi.vercel.app](https://ghibliapi.vercel.app)

## Tags

- Anime
- Studio Ghibli
- Films
- Characters
- Locations
- Species
- Vehicles
- Public APIs
- Open Source
- Read-Only

## Timestamps

- **Created:** 2026-05-28
- **Modified:** 2026-05-29

## APIs

### Studio Ghibli API

Read-only REST API exposing five resource collections (films, people, locations, species, vehicles) that catalog the worlds of Studio Ghibli. No authentication; default page size 50, max 250; optional `fields=` projection.

- **Human URL:** [https://ghibliapi.vercel.app](https://ghibliapi.vercel.app)
- **Base URL:** `https://ghibliapi.vercel.app`

#### Tags

- Anime
- Studio Ghibli
- Films
- Characters
- Locations
- Species
- Vehicles

#### Properties

- [Documentation](https://ghibliapi.vercel.app)
- [OpenAPI](openapi/studio-ghibli-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/studio-ghibli.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/studio-ghibli.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/studio-ghibli-film-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/studio-ghibli-person-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/studio-ghibli-location-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/studio-ghibli-species-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/studio-ghibli-vehicle-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Structure](json-structure/studio-ghibli-film-structure.json)
- [JSON Structure](json-structure/studio-ghibli-person-structure.json)
- [JSON Structure](json-structure/studio-ghibli-location-structure.json)
- [JSON Structure](json-structure/studio-ghibli-species-structure.json)
- [JSON Structure](json-structure/studio-ghibli-vehicle-structure.json)
- [Example](examples/studio-ghibli-listfilms-example.json)
- [Example](examples/studio-ghibli-getfilm-example.json)
- [Example](examples/studio-ghibli-listpeople-example.json)
- [Example](examples/studio-ghibli-getperson-example.json)
- [Example](examples/studio-ghibli-listlocations-example.json)
- [Example](examples/studio-ghibli-getlocation-example.json)
- [Example](examples/studio-ghibli-listspecies-example.json)
- [Example](examples/studio-ghibli-getspecies-example.json)
- [Example](examples/studio-ghibli-listvehicles-example.json)
- [Example](examples/studio-ghibli-getvehicle-example.json)
- [Plans](plans/studio-ghibli-plans-pricing.yml)
- [Rate Limits](rate-limits/studio-ghibli-rate-limits.yml)
- [Authentication](https://github.com/janaipakos/ghibliapi#getting-started)

## Common Properties

- [Website](https://ghibliapi.vercel.app)
- [GitHub Repository](https://github.com/janaipakos/ghibliapi)
- [License](https://github.com/janaipakos/ghibliapi/blob/master/LICENSE)
- [Public APIs Listing](https://github.com/public-apis/public-apis)
- [J S O N- L D](json-ld/studio-ghibli-context.jsonld)
- [Spectral Rules](rules/studio-ghibli-rules.yml)
- [Vocabulary](vocabulary/studio-ghibli-vocabulary.yml)
- [SDK](https://github.com/sotojuan/ghibli)
- [SDK](https://github.com/Rchristiani/totoro)
- [SDK](https://github.com/kisscool-fr/ghibliql)
- [SDK](https://github.com/onertipaday/ghibliapi)
- [SDK](https://github.com/Incognito/python_studio_ghibli_api_sdk)
- [Code Examples](https://github.com/kxvn-lx/Ghibliii)
- [Code Examples](https://github.com/txemasv/ghibli-films)
- [Code Examples](https://github.com/janaipakos/ghibliapi-example)
- [Code Examples](https://github.com/mazipan/ghibli-fans)
- [Code Examples](https://github.com/taniarascia/sandbox/tree/master/ghibli)
- [Features](undefined)
- [Use Cases](undefined)
- [Integrations](undefined)
- [Solutions](undefined)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
