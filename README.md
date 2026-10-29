# C6 Guard updates

Public DNS filter artifacts and signed app-only firmware for C6 Guard. Firmware source and signing private keys remain private.

Catalog: https://luuhung93.github.io/esp32-c6-guard-filters/catalog.json

The manifest binds the catalog by SHA-256. Each catalog entry binds its immutable binary and references the corresponding original source input.

Sources: Guard Starter (CC0), AdGuard DNS filter (GPL-3.0), hostsVN (MIT). See catalog license links and the licenses directory. Original source snapshots are in sources/.

Updates are published by the repository owner after validation. Devices retain already installed lists if downloads are unavailable.

## Firmware updates

Latest release metadata: https://luuhung93.github.io/esp32-c6-guard-filters/firmware/latest.json

Only immutable signed app images are stored in firmware/. C6 Guard 0.2.0+ can check this feed and download an update over Wi-Fi from Settings → Firmware OTA. Each device verifies byte count, SHA-256, native chip/RSA signature, and expected application build before activation. File upload OTA remains available. Never use an app image as a full factory flash set. Keep power on during updates.

The initial online-capable bootstrap is 0.2.0; 0.2.1 is the first feed release for the end-to-end update check. Old digest-named app files stay immutable.
