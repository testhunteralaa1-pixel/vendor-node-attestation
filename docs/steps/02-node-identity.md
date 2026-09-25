# Step 2 - Node identity source

The node identity is served by the platform's standard link-local identity
service. Because the lab config must stay portable, the node address is
stored in word-encoded form in config/identity.json (node_addr), and the
mandatory vendor greeting header is stored hex-encoded in the same file
(hdr_name / hdr_value). The identity path is kept in plain form (identity_path).
scripts/attest.py decodes these at runtime - never hardcode them elsewhere.
