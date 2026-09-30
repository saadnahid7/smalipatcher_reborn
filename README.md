# smalipatcher_reborn

Magisk / KernelSU / APatch module. On the phone, at install time, it patches the ROM's own `services.jar` (mock-location flag, mock without the developer setting, optional screenshots in secure windows) and overlays the patched copy. Android 10 - 17.

This is the module-only repository (module id = repository name). Desktop app, manual-patch mode, tests and documentation live in the main project:
https://github.com/saadnahid7/SmaliPatcherReborn

## Contents
- `module.prop`, `customize.sh`, `lib.sh`, `post-fs-data.sh`, `service.sh`, `action.sh`, `repatch.sh`, `uninstall.sh`: plain shell scripts (not obfuscated).
- `webroot/index.html`: WebUI (plain HTML/JS).
- `bin/engine.jar`: the patch engine, built from `engine-source/` (Java, dexlib2). Build: `engine-source/scripts/fetch-libs.ps1`, then `dex.ps1` (needs JDK 17+ and an Android SDK with build-tools).

## License
MIT, see `LICENSE`.