# 27-Oct-2026

## `vendor/apn`
- apn: Support Python 3.8 (`7693bb9`, Nolen Johnson)

# 26-Oct-2026

## `device/qcom/sepolicy_vndr/sm8750`
- sepolicy_vndr: Restore rules for non init.rc lowi-server (`b25101da`, ExNihilo)

## `hardware/lineage/interfaces`
- fingerprint: aidl: Allow customizing the per-user store path (`68dca0c`, Michael Bestas)

## `hardware/qcom-caf/sm8450/audio/pal`
- pal: Add an option to prefer master gain for equal channel volumes (`2b80768e`, Josip Kelecic)

# 25-Oct-2026

## `device/qcom/sepolicy_vndr/legacy-um`
- sepolicy_vndr: Label nfc2 nxp HAL (`d8b5ffdf`, LuK1337)

## `hardware/lineage/compat`
- compat: Add shim to provide ion_close with proper close(fd) (`f67ba75`, AdarshGrewal)

## `hardware/qcom-caf/sm8750/display/hal`
- display: init: add soc-id support for Kera IoT SoC variants (`5b970807e`, Bhasker Reddy Komatireddy)
- init: add socid for kera (`c4aa37070`, Chintankumar Savaliya)

# 23-Oct-2026

## `device/lineage/sepolicy`
- atv: Add common rules for Netflix app (`a29110e`, Bruno Martins)

## `external/conscrypt`
- Update blocklist (`98b584274`, Luca Stefani)
- Don't require a trailing comma (`1631d45bc`, Luca Stefani)
- Update awk script for new array size names (`256334946`, Luca Stefani)

## `hardware/lineage/interfaces`
- fingerprint: aidl: Log sensor id in getSensorProps (`13281f8`, Michael Bestas)
- health: batteryless: Uprev to version 5 (`9866a16`, Aaron Kling)

## `hardware/qcom-caf/sdm660/audio`
- hal: Stop compress VoIP PCM when the call is kept alive (`0e07d71fe`, LuK1337)

## `packages/apps/Aperture`
- Aperture: Support QHD video quality (`e4fc829`, Mathias Gluszczynski)

# 21-Oct-2026

## `vendor/apn`
- apn: Remove profiles with unlisted MCC/MNC pairs (`c270ee3`, dianlujitao)
- apn: Merge upstream profiles at build time (`a764d38`, dianlujitao)
- apn: Import Pixel APN snapshot (`cfcbd9d`, dianlujitao)

# 20-Oct-2026

## `external/conscrypt`
- Remove emSign Root TLS CA - G3 (`5ea9f383f`, Luca Stefani)
- Remove emSign ECC Root CA - C3 (`e3a6b344c`, Luca Stefani)
- Remove emSign Root CA - C1 (`b4dafc015`, Luca Stefani)
- Update cert blocklist (`d4594bf5c`, Luca Stefani)

## `frameworks/base`
- DisplayManager: Add requestMaxRefreshRate() API (`044b965aa2d3`, LuK1337)

## `system/ca-certificates`
- Remove emSign Root TLS CA - G3 (`3eafa75`, Luca Stefani)
- Remove emSign ECC Root CA - C3 (`c1dab03`, Luca Stefani)
- Remove emSign Root CA - C1 (`114629c`, Luca Stefani)

# 19-Oct-2026

## `frameworks/base`
- SystemUI: show location indicator for OP_COARSE_LOCATION (`ebc25c0cf9c8`, inthewaves)

## `hardware/qcom-caf/common`
- common: Update matrix to LA.QSSI.17.0.r1-11300-qssi.0 (`c7eda1f`, Saalim Quadri)

## `vendor/qcom/opensource/power`
- power: Bump power HAL VINTF fragment to v7 (`2a237fa`, Alexander Koskovich)
- power: Add support for multiple DT2W nodes (`b464d90`, Bruno Martins)
