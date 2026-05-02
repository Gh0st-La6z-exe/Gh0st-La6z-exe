<div align="center">

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=24&duration=4600&pause=1500&color=7AA2F7&center=true&vCenter=true&multiline=true&repeat=true&width=900&height=170&background=1A1B26&lines=Matthew+Morris+%7C+Gh0st-La6z-exe;AI+Software+Engineering+%2B+Cybersecurity;Detection+Systems+%C2%B7+Rust+%C2%B7+Go+%C2%B7+Python+%C2%B7+TypeScript;Building+serious+infrastructure+for+serious+teams" alt="Introduction" />

<p>
  <a href="https://www.linkedin.com/in/nullai"><strong>LinkedIn</strong></a>
  ·
  <a href="https://github.com/Gh0st-La6z-exe"><strong>GitHub</strong></a>
  ·
  <a href="https://www.linkedin.com/in/nullai"><strong>Writing</strong></a>
</p>

</div>

---

## Professional Summary

AI software engineering and cybersecurity practitioner focused on production detection systems, low-latency telemetry, and operator-ready control planes. Most active work is private; I collaborate with teams that value rigorous engineering, measurable security outcomes, and clean system design.

## Stack at a glance (NuLLAI + Abaddon)

Stack map below is sourced strictly from documented NuLLAI + Abaddon components.

<div align="center">

**Row 1/4 · Languages, API, UI**

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Go](https://img.shields.io/badge/Go-00ADD8?style=flat-square&logo=go&logoColor=white)
![Rust](https://img.shields.io/badge/Rust-000000?style=flat-square&logo=rust&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![Tailwind](https://img.shields.io/badge/Tailwind-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white)

**Row 2/4 · Data, Infra, Observability**

![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white)
![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?style=flat-square&logo=prometheus&logoColor=white)
![Grafana](https://img.shields.io/badge/Grafana-F46800?style=flat-square&logo=grafana&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)

**Row 3/4 · Backend and ML libraries**

![Uvicorn](https://img.shields.io/badge/Uvicorn-0B7285?style=flat-square)
![Gunicorn](https://img.shields.io/badge/Gunicorn-499848?style=flat-square&logo=gunicorn&logoColor=white)
![SQLAlchemy](https://img.shields.io/badge/SQLAlchemy-D71F00?style=flat-square&logo=sqlalchemy&logoColor=white)
![Pydantic](https://img.shields.io/badge/Pydantic-E92063?style=flat-square&logo=pydantic&logoColor=white)
![Alembic](https://img.shields.io/badge/Alembic-6B4F1D?style=flat-square)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![scikit--learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white)
![XGBoost](https://img.shields.io/badge/XGBoost-016093?style=flat-square)

**Row 4/4 · Security, Controls, AI Security**

![OpenTelemetry](https://img.shields.io/badge/OpenTelemetry-000000?style=flat-square&logo=opentelemetry&logoColor=white)
![NATS](https://img.shields.io/badge/NATS-27AAEE?style=flat-square)
![JWT](https://img.shields.io/badge/JWT-000000?style=flat-square&logo=jsonwebtokens&logoColor=white)
![mTLS](https://img.shields.io/badge/mTLS-3949AB?style=flat-square)
![HMAC--SHA256](https://img.shields.io/badge/HMAC--SHA256-455A64?style=flat-square)
![OWASP LLM Top 10](https://img.shields.io/badge/OWASP-LLM%20Top%2010-111827?style=flat-square)
![MITRE ATLAS](https://img.shields.io/badge/MITRE-ATLAS-5B21B6?style=flat-square)
![Hugging Face Recon](https://img.shields.io/badge/Hugging%20Face-Recon-FF9D00?style=flat-square&logo=huggingface&logoColor=black)

</div>

## Flagship Platform: NuLLAI XDR

NuLLAI is a **private** autonomous XDR platform that moves security operations from detect-and-alert into a guarded detect-reason-respond pipeline.

It is built to reduce manual SOC correlation by combining telemetry normalization, deterministic enrichment, risk modeling, policy evaluation, and controlled response execution under explicit human override.

**Architecture at a glance**

- **Endpoint layer (`null-agent`, Go):** static cross-platform agent design for telemetry, survivability (WAL), secure transport, and staged kernel-aware observability (eBPF LSM direction).
- **Detection acceleration (`null-detection-core`, Rust + PyO3):** hot-path engines for beaconing, JA3/JA4, DNS tunnel/DGA, IOC/Sigma, baselines, and hunt flows.
- **Control plane (`null-backend`, FastAPI):** tenant-aware orchestration for authz, enrichment, policy checks, incident lifecycle, and autonomous execution control.
- **SOC experience (`null-soc-dashboard`, Next.js/TS):** analyst-facing visibility and controls for incident triage, mode state, and response transparency.

**Telemetry -> Decision -> Action**

Endpoint events -> secure ingestion -> feature extraction and multi-stage scoring -> correlation and MITRE enrichment -> policy and autonomy mode evaluation -> guarded XDR response or block -> full timeline/audit trace.

## Private Program: Abaddon (Adversarial AI Security)

Abaddon is a **private** adversarial AI/ML red-team platform in active rebuild for scoped, authorized testing of ML/LLM systems.

It unifies static artifact auditing, active adversarial workflows, reconnaissance, calibration-focused evaluation, and campaign orchestration so teams can quantify exploitability and remediation confidence.

**Capability pillars**

- **Static and supply-chain auditing:** format-aware analyzers for pickle, safetensors, GGUF, ONNX, Keras, joblib/NumPy surfaces, plus HF recon and dependency CVE checks.
- **Active attack arsenal:** standardized atomics for jailbreak/prompt injection, adversarial examples, poisoning, extraction, and RAG/agent attack paths.
- **Agentic orchestration:** campaign loops with adaptive technique selection, optimization cycles, memory/state, and threat-taxonomy coverage tracking.
- **Recon and serving probes:** stack-aware probing across modern serving surfaces (e.g., TorchServe/Triton/vLLM/TGI/MLflow-style patterns).
- **Evaluation rigor:** calibration-aware scoring, reproducibility-focused reporting, and reliability-oriented statistical testing.

**CLI-first operator flow**

```bash
abaddon atomics list
abaddon atomics run AAR-0001 --scope-file scope.example.yaml --dry-run --allow-high-risk
abaddon scan-artifact path/to/model.safetensors --report ./out
abaddon orchestrate TARGET --scope-file scope.yaml --attacker-model claude-sonnet
```

## Guardrails and Governance

Both NuLLAI and Abaddon are designed around constrained autonomy and auditable safety controls:

- **Scope and tenancy boundaries:** strict tenant isolation and scope allowlisting for target interaction.
- **Mode gating:** explicit autonomy modes with operator-controlled transitions.
- **Execution gating:** dry-run/simulation/live-style checks before potentially disruptive action paths.
- **Kill-switch control:** immediate human override for autonomous response chains.
- **Fail-closed defaults:** out-of-scope or invalid states block execution by design.
- **Auditability:** timeline and decision traces preserved for review, remediation, and governance.

## Engineering Maturity and Documentation

I treat documentation as a first-class engineering artifact across private programs:

- architecture/data-flow specs,
- API and contract documentation,
- operational runbooks (deploy/rollback/incident),
- phase plans with acceptance criteria,
- security and test evidence for auditability.

**Maturity framing:** these are serious platform programs with strong decomposition, testing, and operations discipline. Some subsystems are still evolving (for example, deeper staged eBPF semantics), and that boundary is documented explicitly rather than hidden.

**Scale snapshot (reported in project materials)**

- 870+ API endpoints
- 54 detection engines
- 9 Rust detection crates
- 57 database tables
- 2,700+ backend tests
- 431 Go agent tests
- 618 Rust tests
- Cross-platform endpoint binary targets (Linux/Windows/macOS, amd64/arm64 matrix)

## Signature Capabilities

- **Detection engineering:** Rust-first signal processing, IOC matching, DNS tunneling analysis, JA3/JA4 workflows, and threat-hunt pipelines.
- **Agent architecture:** Linux-focused Go agents with eBPF instrumentation, NATS transport, and no-CGO static binary delivery.
- **Secure backend systems:** FastAPI services with SQLAlchemy and Pydantic, hardened auth patterns (JWT, mTLS, HMAC), and observability-first design.
- **ML and explainability:** PyTorch and classical ML systems with SHAP/LIME support for transparent decisioning.
- **Operational UX:** Next.js and React control planes for real-time visibility, triage, and analyst workflows.

## Technical Stack (Project-Split, Used-Only)

### NuLLAI Stack

- **Endpoint agent (`null-agent`, Go):** Go 1.22/1.24 track, cilium/ebpf, nats.go, x/sys, x/crypto, static no-CGO binary model, WAL survivability.
- **Detection acceleration (`null-detection-core`, Rust):** Rust workspace crates (`beaconing`, `ja3`, `ja4`, `dns_tunnel`, `ioc_matcher`, `sigma`, `behavior_baseline`, `threat_hunt`, `yara`), PyO3 bridge, criterion benchmarks, maturin builds.
- **Control plane (`null-backend`, Python/FastAPI):** FastAPI, Uvicorn, Gunicorn, SQLAlchemy, Pydantic, Alembic, JWT stack (python-jose/PyJWT), cryptography.
- **ML and scoring pipeline:** PyTorch, scikit-learn, xgboost, SHAP, LIME, imbalanced-learn, NumPy, joblib.
- **SOC dashboard (`null-soc-dashboard`):** Next.js, React, TypeScript, Tailwind, ESLint, PostCSS, SWR, recharts, lucide-react.
- **Ops and observability:** PostgreSQL, Redis, Prometheus, OpenTelemetry, Docker/Compose, NATS, Locust.
- **Security controls:** mTLS, HMAC-SHA256, eBPF LSM direction, tenant isolation, mode/kill-switch gating, audit timelines.

### Abaddon Stack

- **Core platform and CLI:** Python package/CLI architecture with scoped command workflows (`atomics`, `scan-artifact`, `scan-hub`, `probe-serving`, `attack`, `orchestrate`).
- **Static and supply-chain auditing:** pickle abstract-VM approach, safetensors, GGUF, ONNX graph analysis, Keras serialized code pattern checks, joblib/NumPy loading-surface checks.
- **Recon and environment analysis:** Hugging Face repository reconnaissance, OSV/CVE-oriented dependency checks, serving-surface probes (TorchServe, Triton, vLLM, TGI, MLflow-style patterns).
- **Adversarial campaign system:** atomics library, technique execution/capture, adaptive orchestration loops (bandit-style selection, optimization cycles, memory/state).
- **Evaluation and reliability science:** calibration-aware scoring, agreement/confidence quality controls, statistical primitives, reproducible reporting and benchmark discipline.
- **Safety model:** scope-file allowlisting, fail-closed validation, constrained serialization paths, no arbitrary eval/exec.

### Shared Overlap (NuLLAI + Abaddon)

- **Languages and runtimes:** Python, Go, Rust, TypeScript.
- **Security engineering model:** constrained autonomy, explicit policy gates, fail-closed defaults, auditability-first design.
- **Data/infra patterns:** containerized services, observable pipelines, reproducible CI-focused engineering posture.
- **Documentation discipline:** architecture specs, runbooks, acceptance criteria, and evidence-backed quality gates.

## Adversarial Methods Coverage

- **Jailbreak and prompt-injection families:** PAIR, TAP, Crescendo, BoN, MSJ, AutoDAN, GCG, ArtPrompt, ReNeLLM, DeepInception, Skeleton Key, PAP, Cipher, indirect injection paths.
- **Adversarial examples:** PGD, C&W, AutoAttack, Square Attack, HopSkipJump.
- **Poisoning and corruption scenarios:** BadNets-style and PoisonedRAG-style workflows.
- **Extraction and leakage testing:** Knockoff Nets style extraction, LiRA-style membership inference, training-data extraction probes.
- **Agent and RAG attack surfaces:** tool-use manipulation, memory/context poisoning, retrieval abuse, and orchestration-path exploitation attempts.
- **Coverage mapping:** OWASP LLM Top 10 and MITRE ATLAS-aligned tracking in campaign/reporting workflows.

## Current Build Themes

- High-throughput detection and analytics pipeline architecture.
- Lightweight endpoint agent and transport-layer engineering.
- Secure decisioning APIs with integrated model explainability.
- Real-time operator dashboards for cyber workflows.

## Writing

Long-form writing and newsletter updates: [**LinkedIn / nullai**](https://www.linkedin.com/in/nullai)
