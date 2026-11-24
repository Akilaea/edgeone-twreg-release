# EdgeOne TW_REG Release Channel

Public update channel for **TW_REG_MAKERS_V1** used by EdgeOne Manager.

- Latest manifest: `latest.json` (raw: https://raw.githubusercontent.com/xbox-cn/edgeone-twreg-release/main/latest.json)
- Stable manifest endpoint: https://api.github.com/repos/xbox-cn/edgeone-twreg-release/contents/latest.json?ref=main
- Latest release: v2.2.0
- Release zip: `TW_REG_MAKERS_V1_v2.2.0.zip`
- Deploy zip: `project.zip` (project files at archive root)
- SHA256: see `SHA256SUMS` / `latest.json`

## v2.2.0
- `POST /batch` runs 5 workers continuously until the container ends.
- `rounds=0`, `seconds=0` by default; one request starts the loop.
- Engine auto-switches between ruyijs and Tanuki on repeated zero-success 5025 rounds.

This repository is the TW_REG package channel only. EdgeOne Manager application self-updates from `xbox-cn/edgeone-manager-release`.
