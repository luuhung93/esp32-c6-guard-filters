# C6 Guard updates

Public DNS filter artifacts and signed app-only firmware for [ESP32-C6 Guard Community](https://github.com/luuhung93/esp32-c6-guard-community). Original project source is GPL-3.0-only; upstream filter data retains its own licenses. Signing private keys and device credentials are never published.

## Filter data

- Legacy catalog: https://luuhung93.github.io/esp32-c6-guard-filters/catalog.json
- Browser country discovery: https://luuhung93.github.io/esp32-c6-guard-filters/catalog/v2/index.json
- Source availability and licenses: [COUNTRY-FILTERS.md](COUNTRY-FILTERS.md), `licenses/` and the catalog links.

AdAway is the default starter; country lists include hostsVN. Devices support up to five installed lists. Installation means ON; Off/remove deletes its local data. Source snapshots remain in `sources/`; immutable filter binaries stay in `filters/`. Some older artifacts/notices are retained for compatibility and do not imply current discovery availability.

Updates are published by the owner after validation. Existing installed policy remains available when downloads fail. Each catalog entry binds its binary by SHA-256 and references original source input; the root manifest binds the legacy catalog.

## Firmware OTA

Latest metadata: https://luuhung93.github.io/esp32-c6-guard-filters/firmware/latest.json

From Settings → Firmware OTA, check for updates and install over Wi-Fi. The ESP validates byte count, SHA-256, native chip/RSA signature and expected application build before activation. Manual app-only upload remains available. Keep power connected during updates; an app image is not a first-install factory flash set.

Version **0.2.19 Community Beta** reduces DNS per-query heap allocations, handles filter/job/OTA JSON allocation failures explicitly, rejects malformed mutation JSON, bounds filter downloads and validates persisted My Rules records. No persistent schema or filter-cap change is included. It uses the retained official signing identity so existing official devices can upgrade.

This is a test release for real LAN/load testing. Long-term multi-device stability, power-loss recovery and the full OTA rollback matrix remain pending. Source, installation instructions, notices and factory packages are in the [community repository releases](https://github.com/luuhung93/esp32-c6-guard-community/releases).

Old digest-named app files stay immutable. CI/self-built images use separate signing identities and are not upgrades for existing official installations.
