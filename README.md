# SAE — State Aware Engine

**SAE (State Aware Engine)** is a **cross-domain temporal intelligence framework** for discovering, tracking, and reasoning about **latent states and regimes** in sequential data.  
It is powered by **NHSMM (Neural Hidden Semi-Markov Models)** and designed to bridge **research-grade sequence modeling** with **production-ready deployment**.

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


SAE uses **NHSMM as its probabilistic core**, while exposing higher-level abstractions for domain-specific adapters, pipelines, and deployment modes.

---

## Core Use Cases

- **Finance & Trading**  
  Market regime detection, volatility states, adaptive strategy modeling.

- **Cybersecurity & Systems Monitoring**  
  Hidden operational states, anomaly detection, behavior shifts in logs or telemetry.

- **IoT & Industrial Analytics**  
  Predictive maintenance, machine state monitoring, fault regime discovery.

- **Health & Wearables**  
  Activity segmentation, physiological state tracking, anomaly detection.

- **Robotics & Autonomous Systems**  
  Behavior monitoring, task phase detection, safety-critical state transitions.

- **General Temporal AI Research**  
  Neural HSMMs, hybrid probabilistic models, non-stationary sequence learning.

---

## Relationship to NHSMM

- **NHSMM**  
  A modular PyTorch library implementing **neural, context-aware Hidden Semi-Markov Models**.

- **SAE**  
  A **system-level engine** built on NHSMM, providing:
  - domain adapters
  - inference pipelines
  - deployment patterns
  - cross-domain abstractions

SAE treats NHSMM as its **latent state inference backbone**.

---

## Deployment Modes (Planned / In Progress)

- **Cloud / SaaS**  
  Scalable, multi-tenant temporal analytics.

- **On-Prem / Edge**  
  Low-latency, privacy-preserving inference close to data sources.

- **Accelerator-Ready**  
  GPU-first execution with future support for additional backends.

---

## Status

> ⚠️ **Alpha / Early Development**

SAE is under active development.  
APIs, abstractions, and deployment tooling may change before `1.0.0`.

---

## Getting Started

SAE currently relies on **NHSMM** as its core dependency.

```bash
pip install nhsmm
```

---

Higher-level SAE components, adapters, and services will be released incrementally.

---

## Support This Project

Development and research around **NHSMM** are supported via
**GitHub Sponsors**, **Patreon**, **Medium**.

See [FUNDING.md](./FUNDING.md) for details on how to contribute and what support enables.

---

## 🧾 License

This project is released under the **Apache License 2.0** © 2024 **AWA.SI**
For full license terms and conditions, please see the [LICENSE](https://github.com/awa-si/SAE/blob/develop/LICENSE) file

If you use NHSMM in academic work, please cite the repository

---




