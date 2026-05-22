# Contributing to AX-Sync-Architecture

Thank you for your interest in contributing to the AX-Sync-Architecture. To maintain our standard of Deterministic Excellence and prevent systemic entropy, all contributions must strictly adhere to the following protocols.

## 1. Contribution Guidelines

* **Determinism First:** Any proposed change to the ISA or pipeline logic must be mathematically provable. We do not accept contributions that introduce stochastic elements or non-deterministic latency.
* **Lipschitz-Constraint:** All new functional blocks must maintain the global stability constant $L \leq 1.0$. You must provide a formal stability proof for any logic that alters the execution flow.
* **Formal Verification:** Contributions must include formal verification models (e.g., TLA+ or Coq proofs). Submissions without formal verification will be rejected.
* **Zero Dependencies:** The architecture relies on zero external dependencies. The introduction of third-party libraries that compromise the deterministic nature of the core is prohibited.

## 2. Submission Process

* **Fork & Branch:** Create a dedicated feature branch for your proposed improvement.
* **Evidence Submission:** All contributions must include an update to `docs/evidence/` documenting the impact on system stability and cycle-accuracy.
* **Stability-Proof-Hash:** Every Pull Request must include a reference to a verified `STABILITY_PROOF.md` update.
* **Jitter-Report:** Submission of timing-analysis data proving $\sigma = 0$ for the modified execution path.
* **Review:** Submissions undergo rigorous automated verification. If a contribution violates the Lipschitz-constraint or introduces jitter, it will be automatically purged by the Aegis-Infinity filter.

## 3. Code of Conduct

We maintain a professional environment focused on technological sovereignty. Discussions are strictly limited to architecture, formal methods, and hardware performance. Lobbying, non-technical debates, and social noise are considered systemic entropy and will not be tolerated.
