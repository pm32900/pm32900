# Prajwal Moras

Software engineer working on AI infrastructure, LLM inference observability, Kubernetes, and backend systems in Go and Python. Based in India.

## Focus
- Kubernetes-native diagnostics for LLM inference (vLLM, Triton)
- Observability with Prometheus and OpenTelemetry
- Backend services: FastAPI, PostgreSQL/pgvector, REST APIs

## Main project: P95 Labs / Inference Fabric Autopilot (IFA)
[p95labs/ifa](https://github.com/p95labs/ifa) · Creator & Maintainer · Aug 2026 – present · independent open-source project, alpha

A read-only Go diagnostics layer for LLM inference on Kubernetes. It correlates Prometheus runtime telemetry with cluster state (via client-go) and produces 19 coded, evidence-backed findings across 7 rule families.
- Validated against live vLLM 0.28.0 (CPU and one NVIDIA L4), Triton 25.12 (CPU only), and a DCGM-compatible exporter on the L4. Kubernetes discovery is tested end to end in a kind cluster (Kubernetes 1.31) in CI
- Read-only `/api/v1/*` API and `ifa` CLI. Docker + Helm packaging with get/list/watch-only RBAC
- Missing telemetry is reported as missing, never treated as zero
- Removed components that couldn't be defended (a no-op node agent, an invalid Ollama path, static sample outputs) and documented the remaining validation gaps

## Also built
[Personal Knowledge Vault](https://github.com/pm32900/personal-knowledge-vault): a deployment-oriented FastAPI + PostgreSQL/pgvector RAG service with JWT auth, cited answers, Alembic migrations, Docker Compose, GitHub Actions CI, and a retrieval evaluation harness (Precision@K, Recall@K, MRR).

## Open-source contributions
- LlamaIndex [#20767](https://github.com/run-llama/llama_index/pull/20767) (merged): fully local RAG notebook with Chroma and Ollama
- LangChainGo [#1506](https://github.com/tmc/langchaingo/pull/1506) (open): OpenTelemetry callback handler in Go
- OpenLLMetry [#4227](https://github.com/traceloop/openllmetry/pull/4227) (open): FastAPI + LiteLLM tracing sample app
- Haystack Cookbook [#272](https://github.com/deepset-ai/haystack-cookbook/pull/272) (open): advanced local RAG notebook
- Ragas [#2605](https://github.com/vibrantlabsai/ragas/pull/2605) (open): AnswerConsistency metric
- Future AGI [#1964](https://github.com/future-agi/future-agi/pull/1964) (open): surface all key-validated providers in the Add Provider dialog

## Stack
Go · Python · SQL · Bash · Kubernetes · client-go · Helm · Docker · kind · GitHub Actions · Prometheus · OpenTelemetry · vLLM · Triton · FastAPI · PostgreSQL · pgvector

## Links
[p95labs.com](https://www.p95labs.com) · [LinkedIn](https://www.linkedin.com/in/praj-moras/) · prajwalmoras10@proton.me
