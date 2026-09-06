# 04-Sep-2026

## `device/qcom/sepolicy_vndr/legacy-um`
- sepolicy_vndr: kona: Label qcom,pm8150l@5:qcom,leds@d300 (`89590c1c5`, soralis0912)

# 01-Sep-2026

## `packages/apps/Aperture`
- Automatic translation import (`cf1bc0a`, LineageOS Infra)

## `packages/apps/FMRadio`
- Automatic translation import (`9382971`, LineageOS Infra)

## `packages/resources/devicesettings`
- Automatic translation import (`e91c799`, LineageOS Infra)

# 31-Aug-2026

## `packages/modules/Connectivity`
- Revert "Use BPF to block socket creation when restricted" (`12221cef10`, hridaya)
- Revert "Always drop non-VPN ingress in lockdown mode" (`cc2435e993`, hridaya)
- Revert "Firewall: More apps/uids again" (`2af9fc5d0d`, hridaya)

## `system/extras`
- Revert "lpmake: Remove --auto-slot-suffixing support." (`c2e4fff6`, Terminator-J)

## `vendor/custom`
- build: envsetup: Grab kernel LLVM version from vendor/lineage (`b28540c`, LuK1337)

## `vendor/pixel/gms`
- config: unset config_evenDimmerEnabled (`7feb332`, Ashwin Devi Srinivasan)

# 30-Aug-2026

## `device/lineage/sepolicy`
- sepolicy: Label basic USB AIDL HAL service (`6151759`, Yumi Yukimura)

## `frameworks/base`
- Revert "Firewall: Transport-based toggle support (1/3)" (`c189df23681a`, Ashwin Devi Srinivasan)

## `packages/apps/Settings`
- Settings: Relocate status bar icon manager to System (`01e89241a2d`, Ashwin Devi Srinivasan)
- Settings: Relocate Navigation mode preference (`4588e0a5255`, aswin7469)

## `packages/modules/Connectivity`
- Revert "Firewall: Transport-based toggle support (3/3)" (`7e95e4dff4`, Ashwin Devi Srinivasan)

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
- overlays: Import translations for "Status bar" from Pixel (`efeb628`, Ashwin Devi Srinivasan)
- Import Crowdin Translations (`7dbfcc6`, Karan Parashar)
- crowdin: Prepare translation infrastructure (`800d5bd`, Karan Parashar)

## `vendor/lineage`
- Merge branch 'lineage-24.0' of https://github.com/LineageOS/android_vendor_lineage into HEAD (`98a80a84`, lemezohaib)

# 28-Aug-2026

## `system/memory/libion`
- libion: Make available to com.android.npumanager (`abd899d`, ralph950412)

## `vendor/lineage`
- release: Update default Clang version from 22.0.1 to 22.0.2 (`3d3e74fb`, LuK1337)
- build: Use kernel LLVM version from release flags (`32f55df4`, LuK1337)

## `vendor/pixel/gms`
- gms: Enable one-pane layouts for embedded activities for tablets (`560c311`, Ashwin Devi Srinivasan)
