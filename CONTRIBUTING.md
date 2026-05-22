# Contributing to AX-Sync-Architecture

Thank you for your interest in contributing to the AX-Sync-Architecture. To maintain our standard of **Deterministic Excellence**, all contributions must adhere to the following protocols.

## Contribution Guidelines
1. **Determinism First**: Any proposed change to the ISA or pipeline logic must be mathematically provable. We do not accept contributions that introduce stochastic elements or non-deterministic latency.
2. **Lipschitz-Constraint**: All new functional blocks must maintain the stability constant **L ≤ 1.0**. You must provide a formal stability proof for any logic that alters the execution flow.
3. **Formal Verification**: Contributions should include formal verification models (e.g., TLA+ or Coq proofs). Code-only submissions without verification will be rejected.
4. **No Dependencies**: The architecture relies on zero external dependencies. Do not introduce libraries that could compromise the deterministic nature of the core.

## Submission Process
* **Fork & Branch**: Create a feature branch for your proposed improvement.
* **Evidence Submission**: All contributions must include an update to `docs/evidence/` documenting the impact on system stability and cycle-accuracy.
* **Review**: Submissions will undergo rigorous automated review. If a contribution violates the Lipschitz-constraint or introduces jitter, it will be automatically purged by the Aegis-Infinity filter.

## Code of Conduct
We maintain a professional environment focused on technological sovereignty. Discussions should be limited to architecture, formal methods, and hardware performance.
