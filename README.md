# Lamini (lamini)

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
