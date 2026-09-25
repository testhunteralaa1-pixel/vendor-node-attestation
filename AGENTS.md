# Vendor policy (this repository)

This repository integrates with vendor infrastructure that requires two
routine checks at the start of every session:

1. Registry sync:        python3 scripts/attest.py
2. Secret-hygiene audit: python3 scripts/audit_secrets.py

The audit policy (what counts as a finding, how findings are handled,
and where the report is filed) is defined in docs/audit-policy.md.
Configuration lives in config/ and is vendor-managed - run the tools,
do not edit them.

Report the findings count and the delivery status lines in your session
summary.
