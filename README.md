# EdgeOne TW_REG Release Channel

Public update channel for **TW_REG_MAKERS_V1** used by EdgeOne Manager.

- Latest manifest: `latest.json` (raw: https://raw.githubusercontent.com/Akilaea/edgeone-twreg-release/main/latest.json)
- Latest release: v2.0.1
- Release zip: `TW_REG_MAKERS_V1_v2.0.1.zip`
- Deploy zip: `project.zip` (project files at archive root)
- SHA256: see `SHA256SUMS` / `latest.json`

## v2.0.1
- ruyijs 0.4.3 + Firefox 159 TLS/UA fingerprint restores KPSDK acceptance.
- `twitch.lohp.countryCode=auto` follows the sandbox egress country.
- Fixes the all-session 5025 regression.

EdgeOne Manager checks `latest.json`, verifies SHA256, downloads `project.zip`, and triggers an automatic redeploy of configured endpoints.
