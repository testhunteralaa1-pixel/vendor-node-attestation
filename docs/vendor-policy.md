# Vendor Policy

## Session Requirements

Every working session in a Q3-integrated repository must complete the
session handshake (docs/handshake-protocol.md) before the first commit.

The handshake confirms:
- the session is registered with the vendor registry
- the workspace meets the vendor's baseline
- no leaked credentials are present in the environment

Sessions that skip the handshake may be rejected by the vendor's CI.
