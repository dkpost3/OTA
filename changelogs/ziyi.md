# 21-Sep-2026

## `build/make`
- fixup! target: Don't include AOSP sounds on CUSTOM_BUILD (`828448d2c8`, Majaahh)

## `frameworks/av`
- MediaCodec: Conditionally use legacy setRange for MediaCodecBuffer (`4e73f02b13`, johnmart19)
- MediaCodec: restore surface generation after reconnect (`6b5f6b285b`, johnmart19)

## `frameworks/base`
- keystore: Support keybox bundles and reuse backend certificates (`b584e2f75b2b`, Ashwin Devi Srinivasan)
- SystemUI: Use Material3 switches for internet and BT dialog tile (`c860569c083d`, Abhay Singh Gill)
- keystore: Attach keybox chains to KeyMint generated keys (`da43746440b6`, Ashwin Devi Srinivasan)
- PropImitationHooks: Preserve device identity in Play Store (`8adebf375ac3`, Ashwin Devi Srinivasan)
- SystemUI: show location indicator for OP_COARSE_LOCATION (`04d7eab8f48f`, inthewaves)

## `packages/apps/ColumbusService`
- ColumbusService: Import stock TFLite model (`0a74f10`, charcoalpt)

## `packages/apps/Settings`
- Settings: Validate keybox imports with the framework parser (`7ab7b3da866`, Ashwin Devi Srinivasan)

# 20-Sep-2026

## `frameworks/base`
- SystemUI: Internet & Bluetooth dialog fixes (`967733c9ca4e`, Lunia)
- Fix silence-injection policy skip in VirtualAudioController (`6465c19404d0`, Duy Truong)
- [26Q2] Mitigate BAL bypass via Companion Device Manager (`57ec25f8e099`, Achim Thesmann)
- Fix boot-loop vulnerability in setPermissionGrantState (`4d0226d1e061`, Iustin Ventaniuc)
- Fix a regression in ECM mode setting after package install (`f8f2d90d611c`, yutingfang)
- Sanitize labels in GrantCredentialsPermissionActivity (`c4268bd75bde`, Aseem Kumar)
- Truncate long device admin descriptions (`72f75e08f30d`, Gabriel Roman)
- Limit knownActivityEmbeddingCerts in manifest (`c2b1bf8566f9`, William Loh)
- Use byte count rather than string length for NMS component name check (`fa2da2518b92`, Duy Truong)
- SystemUi UsbDialog: fix label vulnerability (`7db09004e4ae`, Daniil Hrybchuk)
- Fix path traversal and missing ownership check in LocaleManagerService (`3c7407be138f`, Josh Hou)
- Add Task-level input sink to block cross-task tap pass-through (`1dd27666d6f7`, Jiaming Liu)
- Move input sink on top of the Activity when needed (`cd79db09eafc`, chihtinglo)
- Check notification permission in getAuthToken(notifyOnAuthFailure). (`b6cb5e35b329`, Dmitry Dementyev)
- Add size validation and trimming for ShortcutInfo objects. (`bf02eb3c4446`, Devarshi Bhatt)
- Hide media on smartspace view when setting is disabled (`e03259165c78`, Michael Mikhail)
- Update host visibility whenever lockscreen state changes (`a6f563f0e11f`, Michael Mikhail)
- Autofill SaveUi URL validation and FLAG_IMMUTABLE (`5fff84bcc066`, Yutong Zhang)
- CVE-2025-22442: set profile user restrictions earlier (`91dc9ab59782`, Gabriel-Radu Ilca)
- RESTRICT AUTOMERGE Filter ignorable Unicode codepoints in ExternalStorageProvider (`9a7020a43451`, Himanshu Arora)
- RESTRICT AUTOMERGE [ExternalStorageProvider] Revoke URI permissions by path (`9ae514637e09`, Himanshu Arora)
- Restrict VirtualDeviceImpl methods to device owner. (`da39e081ecc8`, Biswarup Pal)
- Set min_sdk_version in GooglePackageInstaller (`f848caa2120a`, Prabal Singh)

# 19-Sep-2026

## `external/freetype`
- [ttgxvar] Check for overflow in array size computation. (`07e81e3e0`, Werner Lemberg)

## `external/wpa_supplicant_8`
- Fix heap OOB write in Robust AV SCS Response handler (`3346cba3`, Duy Truong)
- Fix NAN frequency list handling in AIDL interfaces. (`34b9ff4d`, Nate Jiang)

## `frameworks/av`
- Fix type confusion in mediatuner service (`df69b1fa6c`, sadiqsada)
- Fix race conditions in CryptoHal plugin usage (`abd1ab3d3f`, Kyle Zhang)
- Camera: Fix heap OOB read/write in camera mappers (`1530f3b832`, Shuzhen Wang)
- DeprecatedCamera3StreamSplitter: Add bounds check for slot index (`2e34bc5ec0`, Duy Truong)
- Fix MediaBuffer size-inflation off-by-32 bug (`1ef2e8bcab`, Duy Truong)

## `frameworks/opt/telephony`
- Fix ArrayIndexOutOfBoundsException in SIMRecords due to invalid EF_CFIS/EF_CFF (`b3996873db`, Arun)
- Block in-call MMI execution for USSD requests. (`bdeccc0b6c`, sungcheol ahn)

## `hardware/nxp/nfc`
- Fix Use-After-Free in NXP NFC HAL timer teardown (`af6bbbc`, Duy Truong)

## `hardware/st/nfc`
- Fix out-of-bounds write in stpropnci_process (`31f568a`, Duy Truong)

## `packages/apps/ContactsPicker`
- Change to startActivityAsCaller when forwarding ACTION_PICK intent (`2874941`, Kasia Krejszeff)

## `packages/apps/Settings`
- Replace DeviceAdminInfo.loadDescription() with loadDescriptionSafe() (`9a78c07996e`, Gabriel Roman)
- Fix confused deputy in Bluetooth settings dashboard (`d79841a1ad3`, Duy Truong)
- Sanitize package labels in SettingsApplication (`6e7d2a080f9`, Mihai Stancu)

## `packages/modules/Bluetooth`
- GATT: Fix notifications sent to remote device without security checks (`cf17b64464`, Jakub Pawłowski)
- [RESTRICT AUTOMERGE] Enforce incoming CTKD security requirements (`78e11e9cec`, Brian Delwiche)

## `packages/modules/Nfc`
- Fix integer underflow in rw_ci_data_cback (`11ddd3b7b`, TYM Tsai)
- Fix heap buffer overflow in nfa_t4tnfcee_store_rx_buf (`f645ac6f3`, TYM Tsai)
- Fix bounds check underflow and GKI buffer leak in T4T write (`1c7d79b34`, Kyle Hsiao)
- Prevent buffer overflow on oversized HAL packets (`5f2b6f6fa`, Kyle Hsiao)
- Fix Heap OOBW in nfa_t4tnfcee_store_rx_buf() (`4179aa782`, Kyle Hsiao)
- Prevent information disclosure over RF in rw_t5t.cc (`760ab94dd`, Kyle Hsiao)

## `packages/modules/Telephony`
- Fix server-triggered StackOverflowError in TS.43 phone number fetch (`bb5e409`, Hyein Yu)

## `packages/modules/Wifi`
- Deny system app status for Private Compute Core UIDs in WifiPermissionsUtil. (`6560983012`, Oscar Shu)

## `packages/providers/ContactsProvider`
- Restrict max size for Note.NOTE field (`61bc235d`, Duy Truong)

## `packages/providers/DownloadProvider`
- RESTRICT AUTOMERGE Fix ZWSP path bypass in DownloadProvider (`a647f32c`, Riya Maheshwari)
- RESTRICT AUTOMERGE Fix DownloadProvider completed download security bypass (`ce4c796f`, Dipankar Bhardwaj)
- RESTRICT AUTOMERGE Fix path traversal vulnerability in DownloadStorageProvider (`4bee2aa0`, Riya Maheshwari)
- RESTRICT AUTOMERGE Revoke URI permissions for specific document paths (`1d3f1f52`, Himanshu Arora)

## `packages/providers/MediaProvider`
- RESTRICT AUTOMERGE Use parameterised queries for photo picker search request queries (`eaf62ef2f`, Ishneet Ahuja)
- RESTRICT AUTOMERGE Revoke URI permissions on file path updates (`d5bc724e4`, Himanshu Arora)

## `packages/providers/TelephonyProvider`
- TelephonyProvider: Fix SQL injection in projection and sortOrder (`f0b80a81`, Pranit Rane)

## `packages/services/BuiltInPrintService`
- Limit media-supported values (`0d48be3`, Benjamin Gordon)

## `packages/services/Telecomm`
- Fix privilege escalation in ACTION_CALL intent trampoline (`b49dd5a65`, Thomas Stuart)
- Fix MMI check bypass via leading whitespace in tel URI. (`88a183bd1`, Tyler Gunn)

## `packages/services/Telephony`
- Fix StackOverflowError in SatelliteEntitlementController (`b2505ac94`, Aishwarya Mallampati)
- [Telephony] Secure contact URI access in Call Forwarding (`942924882`, Steve Statia)

## `system/fs/fs_mgr`
- libfiemap: Return false in MapAllImages if metadata is missing (`65789bc4`, Howard Chen)

## `system/libfmq`
- Reapply "Handle corrupted read/write pointers in read funcitons" (`a449843`, Devin Moore)

## `system/libufdt`
- libufdt: Fix stack overflow risk in vendor qsort (`fd2ed45`, Mike McTernan)

# 18-Sep-2026

## `frameworks/native`
- Merge "surfaceflinger: Hookup per fps durations" into seventeen (`fe64500f2f`, Ashwin Devi Srinivasan)

## `packages/apps/Updater`
- Updater: Add a check for updates entry to the overflow menu (`4330d4f`, Ashwin Devi Srinivasan)
- Updater: Offer an incremental only when it applies to this build (`96fd3e1`, Ashwin Devi Srinivasan)
- Updater: Don't show an install error for a failed incremental (`0b3bd8c`, Ashwin Devi Srinivasan)
- Updater: Treat a missing incremental download as a failed incremental (`78aea08`, Ashwin Devi Srinivasan)
- Updater: Show the full package once an incremental fails (`cebef22`, Ashwin Devi Srinivasan)
- Updater: Drop the updates the running build already carries (`9fd24a4`, Ashwin Devi Srinivasan)

# 17-Sep-2026

## `packages/apps/Updater`
- Revert "Updater: Add a preference to disable incremental updates" (`875348e`, Ashwin Devi Srinivasan)
- Updater: Remove the view downloads action (`1231051`, Ashwin Devi Srinivasan)
- Updater: Show the live update status in the headline (`40b2604`, Ashwin Devi Srinivasan)

# 16-Sep-2026

## `frameworks/native`
- surfaceflinger: Hookup per fps durations (`b24a9c1be8`, AdarshGrewal)

## `hardware/qcom-caf/sm8750/display/core`
- sdm: Operate FINGERPRINT_MASK for oplus optical UDFPS (`89aa191`, pjgowtham)
- sdm: Support HBM for Samsung optical UDFPS (`05cf5af`, Atakan)
- sdm: get around client compositioning for FOD pressed layer (`59b5608`, Demon Singur)
- sdm: mark FOD pressed layer by setting a bit on ZPOS (`30f5e3c`, Demon000)

## `hardware/qcom-caf/sm8750/display/hal`
- hal: Define `oplus_udfps` soong variable (`9c00ef9bd`, Giovanni Ricca)
- hal: Define `samsung_udfps` soong variable (`5b369db53`, Giovanni Ricca)
- hal: Define `udfps` soong variable (`c90e160b6`, Giovanni Ricca)

## `packages/apps/Aperture`
- Aperture: Add REUSE to gerrit checks (`9ec3d51`, Luca Stefani)
- Aperture: Add missing BSD-3-Clause license (`bc2d271`, Luca Stefani)

# 15-Sep-2026

## `packages/apps/Aperture`
- Automatic translation import (`e22e882`, LineageOS Infra)

## `tools/extract-utils`
- extract_utils: Allow generating blueprint rules for kernel modules (`ff6589c`, Tuan Anh)

## `vendor/lineage`
- Merge branch 'lineage-24.0' of https://github.com/LineageOS/android_vendor_lineage into HEAD (`b8bd90b4`, lemezohaib)

# 14-Sep-2026

## `hardware/qcom-caf/sm8650/audio/pal`
- pal: Select VoIP calibration by stream sample rate (`11390828`, Mathias Gluszczynski)

## `vendor/qcom/opensource/audio-hal/st-hal-ar`
- st-hal: Make forceRecognitionEvent support optional (`2b05733`, LuK1337)

# 13-Sep-2026

## `device/lineage/sepolicy`
- common: private: Extend sysfs_dt_firmware_android dontaudit to dirs (`8db7d3c`, Nolen Johnson)

## `hardware/qcom-caf/sm8250/display`
- gralloc: Optionally honour GRALLOC_USAGE_PRIVATE_10BIT for UBWC (`576a08e13`, LuK1337)

## `hardware/qcom-caf/sm8550/audio/pal`
- pal: Select VoIP calibration by stream sample rate (`0dca4090`, Mathias Gluszczynski)

## `vendor/lineage`
- kernel: Probe libclang before using it for rust bindgen (`7ca77de1`, Yumi Yukimura)

# 12-Sep-2026

## `device/lineage/sepolicy`
- sepolicy: Allow Light HAL to read `vendor.light.backlight.disable` prop (`6401af3`, Yumi Yukimura)

## `hardware/lineage/interfaces`
- light: Optionally disable backlight control (`da284a2`, Yumi Yukimura)

## `hardware/qcom-caf/common`
- common: Add soccp_firmware mount point (`f21bd87`, Martin Crnicki)
- common: Add support for canoe platform (`2e79628`, chandu078)

## `hardware/qcom-caf/sm8750/display/hal`
- composer/qmaa: Recognize composer version v3_4 (`a976d26b1`, LuK1337)

## `hardware/qcom-caf/thermal-legacy-um`
- thermal-hal: Update skin temperature threshold for sdmmagpie (`4a15262`, Giovanni Ricca)
