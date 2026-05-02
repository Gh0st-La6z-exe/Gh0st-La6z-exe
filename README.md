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

## Core Technologies

<div align="center">

**Languages & application layer**

<img src="https://skillicons.dev/icons?i=python,go,rust,ts,react,nextjs,fastapi,tailwind,nodejs,bash,vite&theme=dark&perline=11" alt="Languages and application stack" />

**Data, platform, observability, quality**

<img src="https://skillicons.dev/icons?i=postgres,redis,docker,kubernetes,nginx,prometheus,grafana,linux,git,githubactions,pytorch,eslint&theme=dark&perline=12" alt="Platform, observability, and delivery" />

</div>

## Technical Scope

- **Languages:** Python 3.12, Go 1.24, Rust (Edition 2021 workspace), TypeScript.
- **Backend/API:** FastAPI, Uvicorn, Gunicorn, SQLAlchemy, Pydantic, Alembic, python-jose, PyJWT, cryptography.
- **ML/Data:** PyTorch, scikit-learn, xgboost, SHAP, LIME, imbalanced-learn, NumPy, joblib.
- **Detection workspace:** `beaconing`, `ja3`, `ja4`, `dns_tunnel`, `ioc_matcher`, `sigma`, `behavior_baseline`, `threat_hunt`, `yara`; plus PyO3, criterion, maturin.
- **Infra/Operations:** PostgreSQL, Redis, Docker Compose, Prometheus, OpenTelemetry, NATS, Locust.
- **Networking/Security:** JWT, mTLS, HMAC-SHA256, eBPF LSM, async HTTP pipelines (`httpx`, `aiohttp`, `requests`).

## Advanced Tooling Matrix

- **Model and artifact auditing:** pickle abstract VM analysis, safetensors inspection, GGUF analysis, ONNX graph checks (Tarjan/VF2 style patterns), Keras serialization/code-pattern checks, joblib/NumPy loading-surface analysis.
- **AI supply-chain and package risk:** Hugging Face repo recon, OSV/CVE-oriented dependency auditing, ML-environment package audit flows.
- **Serving-surface reconnaissance:** TorchServe, Triton, vLLM, TGI, and MLflow-adjacent deployment probes.
- **Agent and endpoint runtime tooling:** eBPF LSM direction (`bprm_check_security`), secure transport controls, WAL-backed survivability patterns, static no-CGO distribution strategy.
- **Detection and hunt engines:** JA3/JA4, beaconing, DNS tunnel/DGA, IOC matching, Sigma-style detection, behavior baselining, threat-hunt modules.
- **Evaluation and reliability science:** calibration-oriented scoring, confidence/agreement checks, math/stat reliability primitives, benchmark-budget enforcement, reproducibility-first test posture.

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
