# EdgeOne TW_REG Release Channel

Public update channel for **TW_REG_MAKERS_V1** used by EdgeOne Manager.

- Latest manifest: `latest.json` (raw: https://raw.githubusercontent.com/xbox-cn/edgeone-twreg-release/main/latest.json)
- Stable manifest endpoint: https://api.github.com/repos/xbox-cn/edgeone-twreg-release/contents/latest.json?ref=main
- Latest release: v2.0.2
- Release zip: `TW_REG_MAKERS_V1_v2.0.2.zip`
- Deploy zip: `project.zip` (project files at archive root)
- SHA256: see `SHA256SUMS` / `latest.json`

## v2.0.2
- `POST /reg` supports `continuous: true` and `duration`.
- A detached loop runs batches inside the sandbox and the start request returns immediately.
- No follow-up start request is needed.

## v2.0.1
- ruyijs 0.4.3 + Firefox 159 TLS/UA fingerprint restores KPSDK acceptance.

This repository is the TW_REG package channel only. EdgeOne Manager application self-updates from `xbox-cn/edgeone-manager-release`.
