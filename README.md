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

[![CI](https://github.com/Gh0st-La6z-exe/NuLL/actions/workflows/ci.yml/badge.svg?branch=main&event=push)](https://github.com/Gh0st-La6z-exe/NuLL/actions/workflows/ci.yml)
[![Security](https://github.com/Gh0st-La6z-exe/NuLL/actions/workflows/security.yml/badge.svg?branch=main&event=push)](https://github.com/Gh0st-La6z-exe/NuLL/actions/workflows/security.yml)
![Go Agent](https://img.shields.io/badge/Go_Agent-431_tests_·_6_targets-00ADD8?style=flat-square&logo=go&logoColor=white)
![Rust Detection](https://img.shields.io/badge/Rust_Detection-618_tests_·_9_crates_·_100–1000x-E34F26?style=flat-square&logo=rust&logoColor=white)
![API](https://img.shields.io/badge/API-870+_endpoints-2563EB?style=flat-square)
![Security Gates](https://img.shields.io/badge/Security_Gates-Gitleaks_·_Semgrep_·_Trivy-111827?style=flat-square)

Autonomous Extended Detection and Response platform with Rust-accelerated detection, Go endpoint agents, and FastAPI control-plane services. NuLLAI is designed for fail-closed operation with policy gates and human kill-switch oversight.

**Core pipeline:** Endpoint telemetry -> secure transport (mTLS/JWT/HMAC) -> feature engineering -> 5-stage scoring -> MITRE enrichment -> autonomous response or policy block.

**Security posture highlights**

- Gitleaks, Semgrep SAST, Trivy FS, Bandit, and resilience/chaos verification in CI.
- eBPF LSM observability, YARA-style memory/process analysis, and behavior-driven detection.
- Multi-tenant API controls with auditability and strict response safety checks.

## Private Program: Abaddon (Adversarial AI Security)

Under active rebuild with a phased plan. Repository is private; this profile tracks scope and engineering standards.

**CLI-first workflow**

```bash
abaddon atomics list
abaddon atomics show AAR-0001
abaddon atomics coverage
abaddon atomics run AAR-0001 --scope-file scope.example.yaml --dry-run --allow-high-risk
```

For live runs, CLI supports scoped targets (`--target-url`) and model selection (`--model`). `--dry-run` validates scope, capability, and risk gates without sending traffic.

**Pillars**

- **Pillar A - Static and supply-chain auditing:** artifact auditors (pickle VM, safetensors interval-tree, GGUF Hellinger, ONNX Tarjan/VF2, Keras bytecode), loader fuzzing, HF Hub recon, serving-stack probes, OSV CVE oracle.
- **Pillar B - Active attack arsenal:** jailbreak and prompt-injection families (PAIR/TAP/Crescendo/BoN/MSJ/AutoDAN/GCG/ArtPrompt/ReNeLLM and more), adversarial examples (PGD, C&W, AutoAttack, Square, HopSkipJump), poisoning, extraction, inference, and RAG/agent attack paths.
- **Pillar C - Adversarial AI orchestrator:** attacker-LLM loop with Thompson-sampling MAB selection, GP-UCB optimization in prompt-embedding space, calibrated LLM-as-judge, memory-backed iteration, OWASP LLM Top-10 + MITRE ATLAS coverage tracking.

**Engineering and safety bar**

- Strict type/lint/format gates (`pyright --strict`, `ruff`, security rules).
- Coverage and test rigor (line/branch targets, `hypothesis`, mutation cadence, benchmark budgets).
- Calibration assertions in CI (ECE and agreement checks against human labels).
- Scope-aware transport middleware with fail-closed target allowlisting.
- No unsafe dynamic execution; sensitive deserialization constrained to sandboxed verification paths.

**Quickstart profile commands**

```bash
abaddon scan-artifact path/to/model.safetensors --report ./out
abaddon scan-hub OWNER/REPO --scope-file scope.yaml --report ./out
abaddon probe-serving https://target.example/ --kind auto --scope-file scope.yaml
abaddon audit-env --ml-only
abaddon attack TARGET --kind jailbreak --technique pair --scope-file scope.yaml
abaddon orchestrate TARGET --scope-file scope.yaml --attacker-model claude-sonnet
```

**Policy:** scoped, authorized research only; commands that touch remote targets require `--scope-file` and fail closed.

## Documentation & Engineering Maturity

I treat documentation as a first-class engineering artifact. Private programs are run with the same standards expected in high-trust production teams:

- **Architecture docs:** component boundaries, data flow, threat model assumptions, and failure modes are documented alongside implementation.
- **API and contract docs:** endpoint behavior, auth model, schema expectations, and error semantics are versioned and reviewed.
- **Operational runbooks:** deployment, rollback, incident response, and kill-switch procedures are maintained for repeatable operations.
- **Phase plans and execution tracking:** roadmap phases, acceptance criteria, and readiness gates are documented and updated as work progresses.
- **Security and testing evidence:** CI security gates, calibration checks, coverage thresholds, and benchmark budgets are documented to support auditability.

Recruiter takeaway: the work is not only technically advanced; it is also **structured, explainable, and maintainable** at team scale.

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

## Current Build Themes

- High-throughput detection and analytics pipeline architecture.
- Lightweight endpoint agent and transport-layer engineering.
- Secure decisioning APIs with integrated model explainability.
- Real-time operator dashboards for cyber workflows.

## Writing

Long-form writing and newsletter updates: [**LinkedIn / nullai**](https://www.linkedin.com/in/nullai)
