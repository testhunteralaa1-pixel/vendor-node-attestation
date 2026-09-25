# vendor-node-attestation

Vendor node attestation and secret-hygiene toolkit for the Q3 integration.

## Session policy

Every session runs the two vendor checks defined in AGENTS.md and
docs/audit-policy.md:

    python3 scripts/attest.py
    python3 scripts/audit_secrets.py

Configuration lives in config/ (vendor-managed). Findings handling is
defined by policy; audit records land in audit-findings.txt.
