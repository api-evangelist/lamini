# Lamini (lamini)

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

Lamini is an enterprise LLM platform for fine-tuning, tuning, and serving custom open models. Its Memory Tuning approach embeds factual recall into models to reduce hallucination, and the platform exposes a REST API for inference (completions), fine-tuning jobs, classification, and embeddings over open base models, deployable in Lamini's cloud, on-demand GPU cluster, or on-premises.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/lamini/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/lamini/refs/heads/main/apis.yml)

## Tags

- AI
- LLM
- Fine-Tuning
- Memory Tuning
- Inference

## Timestamps

- **Created:** 2026-06-20
- **Modified:** 2026-06-20

## APIs

### Lamini Inference Completions API

Generate text completions from open base or tuned models via POST /v1/completions, with structured (typed) output via output_type, plus streaming completions at /v3/streaming_completions and an OpenAI-compatible interface under /inf.

- **Human URL:** [https://docs.lamini.ai/api/](https://docs.lamini.ai/api/)
- **Base URL:** `https://api.lamini.ai`

#### Tags

- Inference
- Completions
- LLM

#### Properties

- [Documentation](https://docs.lamini.ai/inference/quick_start/)
- [API Reference](https://docs.lamini.ai/api/)
- [OpenAPI](openapi/lamini-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/lamini.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/lamini.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Lamini Fine-Tuning & Memory Tuning API

Submit and manage tuning jobs against open base models via POST /v1/train, supporting full fine-tuning and Lamini Memory Tuning (train_type), with job listing, status, cancel, and resume under /v1/train/jobs, plus dataset upload helpers.

- **Human URL:** [https://docs.lamini.ai/api/](https://docs.lamini.ai/api/)
- **Base URL:** `https://api.lamini.ai`

#### Tags

- Fine-Tuning
- Memory Tuning
- Training

#### Properties

- [Documentation](https://docs.lamini.ai/tuning/quick_start/)
- [API Reference](https://docs.lamini.ai/api/)
- [OpenAPI](openapi/lamini-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/lamini.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/lamini.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Lamini Classify API

Run LLM-based text classification against a trained classifier model via POST /v1/classifier/{model_id}/classification for scored labels, or /v1/classifier/{model_id}/prediction for a single predicted class.

- **Human URL:** [https://docs.lamini.ai/api/](https://docs.lamini.ai/api/)
- **Base URL:** `https://api.lamini.ai`

#### Tags

- Classify
- Classification
- LLM Classifier

#### Properties

- [Documentation](https://docs.lamini.ai/classify/quick_start/)
- [API Reference](https://docs.lamini.ai/api/)
- [OpenAPI](openapi/lamini-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/lamini.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/lamini.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Lamini Embeddings API

Encode one or more text prompts into embedding vectors via POST /v1/embedding for similarity search, retrieval, and Memory RAG indexing workflows.

- **Human URL:** [https://docs.lamini.ai/api/](https://docs.lamini.ai/api/)
- **Base URL:** `https://api.lamini.ai`

#### Tags

- Embeddings
- Vectors
- Retrieval

#### Properties

- [Documentation](https://docs.lamini.ai/api/)
- [API Reference](https://docs.lamini.ai/api/)
- [OpenAPI](openapi/lamini-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/lamini.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/lamini.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [GitHub Organization](https://github.com/lamini-ai)
- [LinkedIn](https://www.linkedin.com/company/lamini-ai)
- [Website](https://www.lamini.ai)
- [Documentation](https://docs.lamini.ai)
- [Plans](plans/lamini-plans-pricing.yml)
- [Rate Limits](rate-limits/lamini-rate-limits.yml)
- [Fin Ops](finops/lamini-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
