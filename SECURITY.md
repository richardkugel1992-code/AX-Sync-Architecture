# Security Policy

## Supported Versions
The AX-Sync-Architecture maintains strict determinism protocols. Security updates are prioritized to preserve system integrity and the defined Lipschitz-constant (L ≤ 1.0).

## Reporting Vulnerabilities
We treat security as a fundamental architectural requirement. Vulnerabilities or deviations from the deterministic execution model should be reported immediately.

1. **Reporting Protocol**: Send a GPG-encrypted summary of the potential vulnerability to the designated security lead.
2. **Evaluation**: All reports are analyzed via the Aegis-Infinity protocol. If an exploit is identified, the patch will be released with priority 1.
3. **Public Disclosure**: We follow a coordinated disclosure policy. Security patches are merged directly into the core branch after passing the formal verification suite.

## Security Model
The system relies on the **Thermox-Quarantine** isolation model. Any component that compromises the cycle-accuracy or determinism of the pipeline is automatically identified and purged from the execution flow.
