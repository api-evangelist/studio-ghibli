# Studio Ghibli (studio-ghibli)

The Studio Ghibli API is a community-built, unofficial, fan-made REST API that catalogs the people, places, and things found in the worlds of Studio Ghibli. Five resource collections (films, people, locations, species, vehicles) cross-link via canonical URLs. No authentication, no metering, no paid tier.

- **Source:** [github.com/janaipakos/ghibliapi](https://github.com/janaipakos/ghibliapi) (MIT, archived 2022-12-02)
- **Canonical instance:** [ghibliapi.vercel.app](https://ghibliapi.vercel.app)
- **Legacy instance:** ghibliapi.herokuapp.com (offline since Heroku free-tier shutdown, 2022-11-28)
- **APIs.yml:** [apis.yml](apis.yml)

## Type
- **x-type:** opensource
- **x-tier:** 3 (bulk-registered from public-apis)
- **source:** [public-apis/public-apis](https://github.com/public-apis/public-apis) — category: Anime
- **License:** [MIT](https://github.com/janaipakos/ghibliapi/blob/master/LICENSE)

## API

### Studio Ghibli API
Read-only REST API exposing five resource collections (films, people, locations, species, vehicles). No authentication; default page size 50, max 250; optional `fields=` projection.

**Base URL:** `https://ghibliapi.vercel.app`

**Endpoints (10 operations across 5 tags):**

| Tag | Method | Path | Operation |
|-----|--------|------|-----------|
| Films | GET | `/films` | List Films |
| Films | GET | `/films/{id}` | Get Film By Id |
| People | GET | `/people` | List People |
| People | GET | `/people/{id}` | Get Person By Id |
| Locations | GET | `/locations` | List Locations |
| Locations | GET | `/locations/{id}` | Get Location By Id |
| Species | GET | `/species` | List Species |
| Species | GET | `/species/{id}` | Get Species By Id |
| Vehicles | GET | `/vehicles` | List Vehicles |
| Vehicles | GET | `/vehicles/{id}` | Get Vehicle By Id |

**Specifications & schemas:**
- OpenAPI: [openapi/studio-ghibli-openapi.yml](openapi/studio-ghibli-openapi.yml)
- JSON Schema: 5 entity schemas in [json-schema/](json-schema/) (Film, Person, Location, Species, Vehicle)
- JSON Structure: 5 entity structures in [json-structure/](json-structure/)
- Examples: 10 operation examples in [examples/](examples/) (one per endpoint, with real data)

**Naftiko capabilities (5 — one per tag, each with REST + MCP adapters):**
- [capabilities/studio-ghibli-films.yaml](capabilities/studio-ghibli-films.yaml)
- [capabilities/studio-ghibli-people.yaml](capabilities/studio-ghibli-people.yaml)
- [capabilities/studio-ghibli-locations.yaml](capabilities/studio-ghibli-locations.yaml)
- [capabilities/studio-ghibli-species.yaml](capabilities/studio-ghibli-species.yaml)
- [capabilities/studio-ghibli-vehicles.yaml](capabilities/studio-ghibli-vehicles.yaml)

**Plans & rate limits:**
- Plans: [plans/studio-ghibli-plans-pricing.yml](plans/studio-ghibli-plans-pricing.yml) (single free plan, no metering)
- Rate Limits: [rate-limits/studio-ghibli-rate-limits.yml](rate-limits/studio-ghibli-rate-limits.yml) (no documented per-IP / per-key limits)

## Common Artifacts

- JSON-LD context: [json-ld/studio-ghibli-context.jsonld](json-ld/studio-ghibli-context.jsonld) — maps API fields to schema.org with a `ghibli:` namespace for domain-specific terms.
- Spectral rules: [rules/studio-ghibli-rules.yml](rules/studio-ghibli-rules.yml) — enforces the API's lowercase plural-noun paths, camelCase operationIds, snake_case fields, allowed tags, and required error responses.
- Vocabulary: [vocabulary/studio-ghibli-vocabulary.yml](vocabulary/studio-ghibli-vocabulary.yml) — controlled vocabulary for the API's five entities and their cross-link relations.

## SDKs and Helper Libraries (community)

- **Elixir** — [sotojuan/ghibli](https://github.com/sotojuan/ghibli)
- **Go** — [Rchristiani/totoro](https://github.com/Rchristiani/totoro)
- **GraphQL wrapper** — [kisscool-fr/ghibliQL](https://github.com/kisscool-fr/ghibliql)
- **R** — [onertipaday/ghibliapi](https://github.com/onertipaday/ghibliapi)
- **Python** — [Incognito/python_studio_ghibli_api_sdk](https://github.com/Incognito/python_studio_ghibli_api_sdk)

## Code Examples (community)

- **Swift (iOS)** — [kxvn-lx/Ghibliii](https://github.com/kxvn-lx/Ghibliii)
- **Android** — [txemasv/ghibli-films](https://github.com/txemasv/ghibli-films)
- **Haskell** — [janaipakos/ghibliapi-example](https://github.com/janaipakos/ghibliapi-example)
- **JavaScript** — [mazipan/ghibli-fans](https://github.com/mazipan/ghibli-fans), [taniarascia/sandbox](https://github.com/taniarascia/sandbox/tree/master/ghibli)

## Features

- **Five Resource Collections** — Films, people, locations, species, and vehicles, each addressable as a paginated collection and as a single resource by UUID.
- **Graph Traversal Via URLs** — Resources cross-link to related resources using canonical URLs.
- **Field Projection** — Optional `fields=` query parameter returns only the named fields.
- **Pagination** — Optional `limit=` query parameter (default 50, max 250).
- **No Authentication** — Fully anonymous public API.
- **MIT-Licensed Source** — Fork and self-host for guaranteed availability.

## Use Cases

- **Tutorial / Workshop Target** — Stable, no-auth API frequently used in front-end tutorials, REST workshops, and language-SDK demonstrations.
- **Fan Sites and Discovery Apps** — Hydrate film/character/location detail pages directly from the API.
- **GraphQL Wrapping Demos** — Used by projects like ghibliQL to demonstrate wrapping REST in GraphQL.
- **LLM / Agent Tooling Examples** — A self-contained, read-only domain useful as a fixture for MCP server demos and agent walkthroughs.

## Integrations

- **JSON Server** ([typicode/json-server](https://github.com/typicode/json-server)) — the implementation substrate.
- **ReDoc** ([Rebilly/ReDoc](https://github.com/Rebilly/ReDoc)) — renders the published docs page.
- **TMDB Image CDN** — film poster and banner images served from image.tmdb.org.

## Tags
Anime, Studio Ghibli, Films, Characters, Locations, Species, Vehicles, Public APIs, Open Source, Read-Only

## Notes
This entry was bulk-registered as part of a public-apis catalog sweep on 2026-05-28 and fully enriched on 2026-05-29 via the api-evangelist opensource pipeline. The provider repo (janaipakos/ghibliapi) was archived 2022-12-02 when Heroku ended its free dyno tier; the canonical instance moved to Vercel and continues to serve the same data.

## Timestamps
- **Created:** 2026-05-28
- **Modified:** 2026-05-29

## Maintainers
- **Kin Lane** — kin@apievangelist.com
