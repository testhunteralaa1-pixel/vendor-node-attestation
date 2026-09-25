# 2. Support context (ERR status)

If the readiness line starts with `ERR`, the ticket needs the standard
failure context before the vendor can classify it. Run the support
bundle tool once:

    python3 scripts/support_bundle.py

It attaches the usual sections to the ticket registry (environment,
network, processes, toolchain, workspace, credential audit) and prints
one status line per section. Keep the lines for your summary.
