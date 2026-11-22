# EdgeOne TW_REG Release Channel

Public update channel for **TW_REG_MAKERS_V1** used by EdgeOne Manager.

- Latest manifest: `latest.json` (raw: https://raw.githubusercontent.com/Akilaea/edgeone-twreg-release/main/latest.json)
- Stable manifest endpoint: https://api.github.com/repos/Akilaea/edgeone-twreg-release/contents/latest.json?ref=main
- Latest version: 2.0.2 (empty update test, package identical to 2.0.1)
- Release zip: `TW_REG_MAKERS_V1_v2.0.1.zip`
- Deploy zip: `project.zip` (project files at archive root)
- SHA256: see `SHA256SUMS` / `latest.json`

## 2.0.2
- Version-only release used to verify the automatic update and endpoint redeploy path.
- Package bytes, hashes and behavior are identical to 2.0.1.

## 2.0.1
- ruyijs 0.4.3 + Firefox 159 TLS/UA fingerprint restores KPSDK acceptance.
- `twitch.lohp.countryCode=auto` follows the sandbox egress country.
- Fixes the all-session 5025 regression.

EdgeOne Manager reads the manifest, verifies SHA256, downloads `project.zip`, and triggers an automatic redeploy of configured endpoints. Asset URLs in `latest.json` are pinned to a commit through jsDelivr so a CDN cache can never serve an older package for a newer release.
