# 30-Aug-2026

## `device/lineage/sepolicy`
- sepolicy: Label basic USB AIDL HAL service (`6151759`, Yumi Yukimura)

## `vendor/pixel/gms`
- gms: Add accessibility service and ordering configs to GoogleSettingsOverlay (`991faad`, Ashwin Devi Srinivasan)

# 29-Aug-2026

## `frameworks/base`
- SystemUI: Implement reverse-engineered mobile data confirmation dialog (`64ea1bbe8e61`, Ashwin Devi Srinivasan)
- VolumeDialog: Fix layout issues with left gravity (`bc9682043b56`, Dmitrii)
- VolumeDialog: Add overlay-configurable left gravity (`de60be7dac20`, Pranav Vashi)

## `hardware/lineage/interfaces`
- usb: aidl-basic: Initial AIDL HAL (`ecac852`, Yumi Yukimura)
- _frameworks: Import displayservice static lib from `android16-qpr2-release` (`aa8abf0`, Michael Bestas)
- _frameworks: displayservice@1.0: Add framework manifest (`fbb4c37`, Yumi Yukimura)
- _frameworks: Rename from `android.frameworks` to `lineage.frameworks` (`23dc70d`, Yumi Yukimura)
- _frameworks: Import stats from `android16-qpr2-release` (`0a935fe`, Michael Bestas)
- _frameworks: Import displayservice from `android16-qpr2-release` (`5708b39`, Yumi Yukimura)

## `hardware/qcom-caf/common`
- common: Drop no longer used TARGET_COMPILE_WITH_MSM_KERNEL (`2cd569f`, Michael Bestas)

## `packages/apps/Settings`
- fixup! Settings: Implement reverse-engineered expressive QR generator (`2785ba99453`, rwicept)

## `packages/apps/Updater`
- Updater: Move translations to Crowdin (`a3d2202`, Ashwin Devi Srinivasan)
- Updater: Add certified props update support (`01dd671`, Ashwin Devi Srinivasan)

## `vendor/apn`
- FR: Update APN for Free Mobile (`e003409`, Mashopy)
- FR: Update APN for Orange (`c734664`, Mashopy)
- FR: Update APN for Bouygues Telecom (`a57664f`, Mashopy)

## `vendor/crowdin`
- Import Crowdin Translations (`7dbfcc6`, Karan Parashar)
- crowdin: Prepare translation infrastructure (`800d5bd`, Karan Parashar)

# 28-Aug-2026

## `system/memory/libion`
- libion: Make available to com.android.npumanager (`abd899d`, ralph950412)

## `vendor/pixel/gms`
- gms: Enable one-pane layouts for embedded activities for tablets (`560c311`, Ashwin Devi Srinivasan)

# 27-Aug-2026

## `external/chromium-webview/patches`
- Update Chromium Webview to 152.0.7977.64 (`209a6d2`, Kevin F. Haggerty)

## `external/chromium-webview/prebuilt/arm`
- Update Chromium Webview arm to 152.0.7977.64 (`80e8063`, Kevin F. Haggerty)

## `external/chromium-webview/prebuilt/arm64`
- Update Chromium Webview arm64 to 152.0.7977.64 (`a6b2364`, Kevin F. Haggerty)

## `external/chromium-webview/prebuilt/x86`
- Update Chromium Webview x86 to 152.0.7977.64 (`58479e5`, Kevin F. Haggerty)

## `external/chromium-webview/prebuilt/x86_64`
- Update Chromium Webview x86_64 to 152.0.7977.64 (`2767453`, Kevin F. Haggerty)

## `vendor/apn`
- PL: Remove Aster (`eae6025`, Wiktor Rudzki)
- PL: Remove Mobilking and MNI Mobile (`dae435a`, Wiktor Rudzki)
- PL: Remove Era & Tak-Tak (`6f1162e`, Wiktor Rudzki)
- PL: Remove mBank Mobile (`c40ee06`, Wiktor Rudzki)
- PL: Remove PlusWAP (`37974c6`, Wiktor Rudzki)
- PL: Remove GaduAIR (`874c462`, Wiktor Rudzki)
- PL: Remove Carrefour Mova (`5355f6b`, Wiktor Rudzki)

# 25-Aug-2026

## `prebuilts/extract-tools`
- apktool: Update to v3.0.3 (`aaeb969`, LuK1337)

# 24-Aug-2026

## `packages/apps/Updater`
- Updater: Shorten preferences menu entry (`5fc7936`, Ashwin Devi Srinivasan)
- Updater: Enable performance mode by default (`52da21f`, charcoalpt)
- Updater: Pixel-fidelity UI refinements (`1b4aad6`, charcoalpt)

# 23-Aug-2026

## `tools/extract-utils`
- sdat2img.py: Switch shebang line to python3 (`06594f2`, Wiktor Rudzki)

# 22-Aug-2026

## `device/lineage/sepolicy`
- common: private: Don't audit bootanimation searching system_data_file (`b446a7e`, Nolen Johnson)
- atv: Don't audit Katniss cgroup spam (`816baaa`, Nolen Johnson)
- sepolicy: atv: vendor: Don't audit TvSettings reaching into GMS dirs (`a85122e`, Nolen Johnson)

## `packages/apps/Aperture`
- Aperture: Update CameraX to 1.7.0-alpha03 (`88625a9`, LuK1337)

## `packages/apps/Updater`
- Updater: Adapt translations (`8b5fd69`, Ashwin Devi Srinivasan)
- Updater: Adapt updater for PixelOS (`9f729b6`, Ashwin Devi Srinivasan)
- Updater: Use Pixel loading animation (`6f29b07`, AdarshGrewal)
- Updater: Remove superseded settings UI (`0f10268`, AdarshGrewal)
- Updater: Present updates in the system update screen (`b2d0246`, AdarshGrewal)
- Updater: Add Pixel-style system update screen (`31d4a1e`, AdarshGrewal)

## `vendor/apn`
- FR: Update APN for SFR (`dd249f1`, Nolen Johnson)
