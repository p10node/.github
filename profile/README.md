<div align="center">
    <a href="https://p10node.com">
        <img width="256" src="https://raw.githubusercontent.com/p10node/.github/refs/heads/main/images/p10node-logo.svg">
    </a>

  <h3>Software that ships often and stays up.</h3>

  <p>We build, ship and run production systems for teams that cannot afford downtime.<br>
  One senior team, from the first commit to the 3 a.m. pager.</p>

  <a href="https://p10node.com">Website</a> ·
  <a href="https://p10node.com/services">Services</a> ·
  <a href="https://p10node.com/insights">Insights</a> ·
  <a href="https://oss.p10node.com">Open source</a> ·
  <a href="mailto:ping@p10node.com">ping@p10node.com</a>
</div>

---

## ⭐ k10s — the Kubernetes terminal UI you can *click*

[**github.com/p10node/k10s**](https://github.com/p10node/k10s) — k9s taught us to live in the terminal. k10s keeps that, then adds a mouse, one search box for the whole cluster, and an AI that already knows your context, namespace and selected object.

[![stars](https://img.shields.io/github/stars/p10node/k10s?style=flat&logo=github&label=stars)](https://github.com/p10node/k10s)
[![release](https://img.shields.io/github/v/release/p10node/k10s?style=flat&label=release)](https://github.com/p10node/k10s/releases)
[![go](https://img.shields.io/badge/go-1.26%2B-00ADD8?logo=go&logoColor=white)](https://github.com/p10node/k10s/blob/main/go.mod)
[![platforms](https://img.shields.io/badge/platforms-macOS%20%C2%B7%20Linux%20%C2%B7%20Windows-lightgrey)](https://github.com/p10node/k10s#install)
[![license](https://img.shields.io/badge/license-Apache--2.0-blue)](https://github.com/p10node/k10s/blob/main/LICENSE)

```sh
curl -fsSL https://p10node.com/k10s/install.sh | sh
```

- **30 resource kinds** across Workloads, Network, Config, Storage, RBAC, Cluster and Custom Resources, with live row counts. Your CRDs are discovered automatically
- **Day-2 toolkit on single keys** — describe, YAML, follow logs, shell in, port-forward, top, edit, restart, scale, cordon/drain, delete. Your k9s-style `plugins.yaml` shortcuts fit right in
- **One search box for the whole cluster** — `ctrl+p` searches resource kinds and objects in the same result list
- **AI that can see the screen** — `ctrl+a`, ask in plain English. Context, namespace, kind and selected object are injected into the prompt. Bring your own key: OpenAI-compatible or Anthropic
- **Opens instantly** — zero watches at startup, informers wake up lazily per kind
- **Eight built-in themes, plus your own** — tokyo-night, catppuccin-mocha, dracula, nord, gruvbox-dark, solarized-dark, solarized-light, matrix. Drop a YAML palette in `~/.k10s/themes`
- **Single static binary that updates itself** — `k10s update`, checksum-verified and atomic. `k10s demo` for an offline sample cluster, `--readonly` to look and never touch

> If you live in `kubectl`, this is the one repo of ours to star. Coming from k9s? The keymap is in the README.

## More open source

We ship the tools we needed at 3 a.m. Everything built for our own infrastructure gets the same question: would this have saved someone else the night? If yes, it lands here.

|                                                            | Status      | What it is                                                                                                                                                                                       |
|------------------------------------------------------------|-------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **[p10logs](https://github.com/p10node/p10logs)**          | live        | Persistent, multi-cluster Kubernetes pod logs. One DaemonSet agent, one hub with a PVC, built-in UI. No metrics, no Elasticsearch, no Grafana. Go · Apache-2.0 · Helm chart on `ghcr.io/p10node/charts` |
| **[local-rwx](https://github.com/p10node/local-rwx)**      | pre-release | `ReadWriteMany` volumes from the local disk you already have, served over NFS-Ganesha. No replication, on purpose. Go · Apache-2.0 · Kubernetes 1.35+                                            |
| **[listmngr](https://github.com/p10node/listmngr)**        | live        | Mailing-list manager in Rust that replaces GNU Mailman 3 (core, Postorius, HyperKitty): one static binary, SQLite or PostgreSQL, LMTP in, SMTP out, web UI, archive, Mailman 3.1 REST API. AGPL-3.0 |
| **[qcpa](https://github.com/p10node/qcpa)**                | research    | Quantum Computing: Practical Applications. 38 laptop-scale experiments with honest classical baselines, reproducible runs and IBM hardware results. Python                                      |
| **[CropText](https://github.com/p10node/CropText)** · **[SmartRotate](https://github.com/p10node/SmartRotate)** | apps | Small native macOS apps, one job each, nothing leaves your Mac. Swift 6 · SwiftUI · [app.p10node.com](https://app.p10node.com)                                                                   |

Built in public from the first commit. Issues answered by the people who run it.

---

## What we do

|      | Practice                                                                                                                                                                                                        | Works with                                                   |
|------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------|
| `01` | **[Software engineering](https://p10node.com/services#software-engineering)** — greenfield web, API and data platforms, legacy modernisation and service decomposition, architecture and code review, data pipelines and event-driven systems. Built by the engineers who will also run it. | Go · TypeScript · Python · Java · Rust · PostgreSQL · Kafka |
| `02` | **[Deployment & delivery](https://p10node.com/services#deployment)** — CI/CD on GitHub Actions, GitLab CI or Jenkins, GitOps with Argo CD, promotion and preview environments, canary and blue/green rollouts with automatic rollback, supply chain: signing, SBOM, image scanning. | Kubernetes · Argo CD · Helm · Terraform · Docker · Cosign    |
| `03` | **[Infrastructure & monitoring](https://p10node.com/services#infrastructure)** — reliability assessment with a scored roadmap, IaC and multi-region design, SLOs, error budgets and distributed tracing, 24/7 on-call, incident command, blameless reviews. | Prometheus · Grafana · OpenTelemetry · Loki · PagerDuty      |
| `04` | **[AI infrastructure](https://p10node.com/services#ai)** — GPU capacity planning and build-vs-rent strategy, inference clusters, scheduling and autoscaling, RAG and vector store architecture, LLMOps: evaluation, guardrails, unit economics. Cost per thousand requests tracked like any other SLI. | NVIDIA · vLLM · Ray · Kubeflow · Triton · pgvector           |
| `05` | **[Cloud, cost & compliance](https://p10node.com/services#additional)** — cloud migration and data centre exit, FinOps: right-sizing, commitments, budget alerts, disaster recovery design and restore drills, ISO 27001 and SOC 2 readiness, secrets management. | Vault · Trivy · OPA · Velero · FinOps                        |

## Track record

| 99.98%                            | −46%                             | 12 min                         | 140+                            |
|-----------------------------------|----------------------------------|--------------------------------|---------------------------------|
| Average uptime, managed platforms | Median cloud spend cut, year one | Median time to restore service | Environments built and operated |

## How we work

**Assess** (two weeks) → **Architect** → **Automate** → **Operate** (24/7 follow-the-sun cover, 15-minute incident response). Four phases, fixed checkpoints, a named engagement lead for the whole programme, one fixed monthly figure agreed up front.

Work happens in your repositories and your cloud accounts. You own every repo from the first commit, the exit plan is written on day one, and retainers are cancellable with 30 days' notice.

## Insights

- [The three numbers that decide what your inference costs](https://p10node.com/insights/gpu-inference-cost-per-thousand-requests) — cost per thousand requests is an SLI. Batching, utilisation and the tail of your latency distribution set it
- [Cutting cloud spend, in the order that actually works](https://p10node.com/insights/cloud-cost-the-order-we-do-it-in) — reserved instances are real savings, but they are last, not first
- [What a reliability assessment actually looks at](https://p10node.com/insights/reliability-assessment-what-we-look-at) — two weeks inside a production system, and the eight questions that decide the score

More at [p10node.com/insights](https://p10node.com/insights) · [RSS](https://p10node.com/insights/feed.xml)

---

<div align="center">
  <sub>DevOps engineering since 2025. 32 senior engineers in Ho Chi Minh City, serving South-East Asia, Europe and Australia. English and Vietnamese.<br>
  Tell us what is breaking, or what you want to build — a short note reaches an engineer, not a sales sequence.<br><br>
  <a href="https://p10node.com/contact"><b>Book a 30-minute call</b></a><br><br>
  <a href="https://oss.p10node.com">Open source</a> ·
  <a href="https://app.p10node.com">Apps</a> ·
  <a href="https://books.p10node.com">Books</a> ·
  <a href="https://hardware.p10node.com">Hardware</a></sub>
</div>
