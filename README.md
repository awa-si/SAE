# SAE — State Aware Engine

**SAE (State Aware Engine)** is a **cross-domain temporal intelligence framework** for discovering, tracking, and reasoning about **latent states and regimes** in sequential data.  
It is powered by **[NHSMM](https://github.com/awa-si/NHSMM) (Neural Hidden Semi-Markov Models)** and designed to bridge **research-grade sequence modeling** with **production-ready deployment**.

SAE provides a unified engine for **state inference, regime detection, and temporal decision support** across heterogeneous, non-stationary time series.

---

## Key Capabilities

- **Explicit Latent State Modeling**  
  Models hidden regimes with **variable, learnable state durations**, enabling accurate dwell-time reasoning beyond standard HMMs.

- **Context-Aware Dynamics**  
  Initial states, transitions, durations, and emissions can be **modulated by external covariates**, supporting non-stationary and adaptive behavior.

- **Neural + Probabilistic Hybrid**  
  Combines **classical HSMM structure** with **neural parameterization**, preserving interpretability while increasing expressiveness.

- **Exact and Approximate Inference**  
  Supports forward-backward likelihoods, Viterbi decoding, and differentiable training for neuralized latent states.

- **Production-Oriented Design**  
  GPU-ready, batched, modular, and suitable for cloud, on-prem, or edge deployment.

---

## Relationship to [NHSMM](https://github.com/awa-si/NHSMM)

- **NHSMM**  
  A modular PyTorch library implementing **neural, context-aware Hidden Semi-Markov Models**, fully **open-source**.

- **SAE**  
  A **system-level engine** built on NHSMM, providing:
  - domain adapters
  - inference pipelines
  - deployment patterns
  - cross-domain abstractions

SAE treats NHSMM as its **latent state inference backbone**.

---

## Core Use Cases

- **Finance & Trading** — Market regime detection, volatility states, adaptive strategy modeling.  
- **Cybersecurity & Systems Monitoring** — Hidden operational states, anomaly detection, behavior shifts in logs or telemetry.  
- **IoT & Industrial Analytics** — Predictive maintenance, machine state monitoring, fault regime discovery.  
- **Health & Wearables** — Activity segmentation, physiological state tracking, anomaly detection.  
- **Robotics & Autonomous Systems** — Behavior monitoring, task phase detection, safety-critical state transitions.  
- **General Temporal AI Research** — Neural HSMMs, hybrid probabilistic models, non-stationary sequence learning.

---

## Deployment Modes (Planned / In Progress)

- **Cloud / SaaS** — Scalable, multi-tenant temporal analytics.  
- **On-Prem / Edge** — Low-latency, privacy-preserving inference close to data sources.  
- **Accelerator-Ready** — GPU-first execution with future support for additional backends.

---

## Status

> ⚠️ **Alpha / Early Development**

SAE is under active development.  
APIs, abstractions, and deployment tooling may change before `1.0.0`.

---

## Getting Started

SAE currently relies on **NHSMM** as its core dependency:

```bash
pip install nhsmm
Higher-level SAE components, adapters, and services will be released incrementally.
Early-access versions and research previews are available via Patreon or subscription for controlled use.
```

## Licensing
SAE is released under a Proprietary License © 2026 AWA.SI.

The repository is public, but usage is restricted:

Viewing, cloning, and personal experimentation are permitted.

Redistribution, commercial use, or deployment without permission is prohibited.

Early-access releases may be provided to subscribers via Patreon, with copy usage governed by this Proprietary License.

For full license terms, see LICENSE.

NHSMM remains fully open-source (Apache 2.0), and can be used independently.

## Support This Project
Development and research around SAE and NHSMM are supported via:

Patreon (early-access, research sketches, pre-releases)

GitHub Sponsors

Medium articles & research notes

See FUNDING.md for details on how contributions help sustain development.
