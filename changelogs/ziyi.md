# 14-Sep-2026

## `build/make`
- fixup! target: Don't include AOSP sounds on CUSTOM_BUILD (`026d895c1b`, Majaahh)

## `frameworks/base`
- Fix Bluetooth tile dialog subtitle alignment (`4eac95d24f46`, Lunia)
- SystemUI: show location indicator for OP_COARSE_LOCATION (`ec1f7e059942`, inthewaves)

## `hardware/qcom-caf/sm8650/audio/pal`
- pal: Select VoIP calibration by stream sample rate (`11390828`, Mathias Gluszczynski)

## `system/memory/libmeminfo`
- sysmeminfo: Avoid abort when map is missing (`7028eee`, Hridaya Prajapati)

## `vendor/lineage`
- kernel: Probe libclang before using it for rust bindgen (`a5afe97a`, Yumi Yukimura)

# 13-Sep-2026

## `device/lineage/sepolicy`
- common: private: Extend sysfs_dt_firmware_android dontaudit to dirs (`8db7d3c`, Nolen Johnson)

## `hardware/qcom-caf/sm8250/display`
- gralloc: Optionally honour GRALLOC_USAGE_PRIVATE_10BIT for UBWC (`576a08e13`, LuK1337)

## `hardware/qcom-caf/sm8550/audio/pal`
- pal: Select VoIP calibration by stream sample rate (`0dca4090`, Mathias Gluszczynski)

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

## `vendor/lineage`
- Merge branch 'lineage-24.0' of https://github.com/LineageOS/android_vendor_lineage into HEAD (`28ea0917`, lemezohaib)

# 11-Sep-2026

## `vendor/lineage`
- kernel: Wipe bazel dist dir on each build (`dde7a2aa`, Alexander Koskovich)
- kernel: Seperate bazel-out from the dist dir (`0f3eb2d4`, Alexander Koskovich)
- release: Bump Security String to 2026-09-01 (`95bc7319`, Nolen Johnson)
- kernel: Add RBE support (`b104fc7b`, LuK1337)

# 10-Sep-2026

## `packages/apps/Updater`
- Updater: Add a preference to disable incremental updates (`cb812f2`, Ashwin Devi Srinivasan)
- Updater: Support incremental OTA packages (`b07544a`, Ashwin Devi Srinivasan)

## `vendor/lineage`
- kernel: Add AOSP build-tools to inline kernel PATH (`790f1937`, Alexander Koskovich)
- build: Fix typo in kernel.mk (`2116535d`, Tommaso Fonda)

# 09-Sep-2026

## `packages/apps/Updater`
- Updater: Migrate import progress dialog to Jetpack Compose (`848af1b`, Lunia)
- Updater: Use Compose system update icon (`be6fa0c`, Lunia)

## `vendor/lineage`
- vars: Add kaanapali-{audio,video,wlan} (`e7d54ba8`, LuK1337)
- vars: Add kaanapali-vendor (`40ebf64b`, LuK1337)
- Merge commit 'refs/changes/75/497575/3' of https://github.com/LineageOS/android_vendor_lineage into HEAD (`dc91838c`, Ashwin Devi Srinivasan)

# 08-Sep-2026

## `art`
- Make the runtime-generated app image read-only (`03ecb9ce33`, Nicolas Geoffray)

## `development`
- Fix potential NPEs in PduParser.parsePartHeaders (`d36bcc0d6`, Soumyadeep Paul)

## `external/exfatprogs`
- ANDROID: Fix fsck overflows when handling bad clu_count or vol_length fields. (`96fc1f4`, David Anderson)
- ANDROID: Add support for building exfat tests. (`e2e0f4f`, David Anderson)

## `frameworks/av`
- Fix OOB in DynamicsProcessing MBC band processing (`06458fc827`, Duy Truong)
- Fix heap-buffer-overflow in AudioAttributes unmarshalling (`ce3fda8e0e`, Venkatarama Avadhani)

## `frameworks/base`
- aapt2: Sanitize Javadoc comments to prevent code injection (`db291d9dc8bd`, Mark Punzalan)
- Fix potential NPEs in PduParser.parsePartHeaders (`479f93381ad2`, Soumyadeep Paul)
- RESTRICT AUTOMERGE: Fix vulnerabilities in PduParser (`df744839e7b4`, Thomas Nguyen)
- ResStringPool: Validate styleCount and offsets (`54ac9adea408`, Jeremy Meyer)
- Remove CLASS_EXISTENCE_CHECK metadata from ConnectivityCallListenerService (`36f695a8e524`, sungcheol ahn)
- RESTRICT AUTOMERGE Fix security vulnerability in getManageSpaceActivityIntent (`1b5d255eae37`, Yang Kudurshian)
- Validate caller UID in openProxyFileDescriptor (`ab3081a8e44f`, Darshil Shah)
- Add bracket checking support to SQLiteTokenizer (`be310a1d9454`, Duy Truong)
- Fix security check bypass (`dbe5ab03b897`, Duy Truong)
- Strip URI grants in ConfigActivityProxy (`27aa96a5720d`, Taso Dane)
- Fix BAL bypass via getAppMarketActivityIntent (`c56ee3ca39dc`, Himanshu Gupta)
- LauncherApps: Scrub sensitive URIs in install sessions (`c1846ac1e4da`, Prabal Singh)
- Remove usage of Parcel.allowSquashing in RemoteViews and immediate unparceling of Bundle (`5b66d57b6a16`, Vipul Singh)
- Revert^2 "Writing ApplicationInfoCache instead of multiple ApplicationInfos for nested RemoteViews" (`a73e7ac3d7ac`, Vipul Singh)
- Fix using the base type for checking (`03a20093e332`, Candice Lo)
- Properly parse meta_key in AccountsDb. (`ec2c67d49c2d`, Dmitry Dementyev)
- Don't parse 3p recognizer metadata in safe mode (`8309b1c4a01f`, Omar Eissa)
- Dedup SessionParams.whitelistedRestrictedPermissions (`ce1df3fc3017`, William Loh)
- Fix & speed up IntentForwarderActivityTest (`c7a161e13835`, Matt Casey)
- Validate caller in SlicePermissionActivity to prevent spoofing. (`ce41d92a4412`, Yash Nagayach)
- Update URI permission granting logic in Intent Redirection Hardening (`a636a139d48b`, Yang Kudurshian)
- Move intent redirect checks before intent resolution. (`76b5c7ebfdbb`, Nan Wu)
- Fix intent redirect bypass via selector in addCreatorToken (`94193d05a839`, Nan Wu)
- Refactor: Add permission checks to Unarchive activities (`660b383fdce4`, Prabal Singh)
- fix an inverted boolean check (`19b63ba95f8b`, Song Chun Fan)
- Check notification setting for given user (`4c2f227c3430`, Evan Severson)
- Use consistent mmap/unmap sizes in MemoryIntArray (`6d8868becfc1`, Jared Duke)

## `hardware/qcom-caf/thermal`
- thermal-hal: Relax LIGHT and MODERATE skin limits for volcano (`a54c4be`, Rohit Sekhar)

## `packages/apps/Settings`
- Sanitize sensitive BiometricsSettingsBase extra (`cee0f8941ad`, Milton)
- Ensure remote device credential alias is used for action CONFIRM_REMOTE_DEVICE_CREDENTIAL. (`bb425f1964e`, Joe Bolinger)
- Remove EXTRA_DATA from ConfirmDeviceCredentialActivity (`e29fdcb7fac`, Diya Bera)
- Strip URI grant flags in AppRestrictionsFragment (`5026849b1da`, Tetiana Meronyk)
- Remove dialog building logic from PaymentDefaultDialog onCreate. (`6a06dace2b1`, Kyle Hsiao)

## `packages/modules/Bluetooth`
- Fix buffer overflow in UUID parsing (`4f36f54dd8`, Brian Delwiche)
- Fix out-of-bounds heap write in SnoopLogger (`6a2bf1d22a`, Brian Delwiche)
- Fix cross-thread UAF in AvrcpService updates (`fc76a3ad5a`, Brian Delwiche)
- Fix uninitialized pointer dereference in MsftExtensionManager (`18eea5b9e1`, Brian Delwiche)

## `packages/modules/Nfc`
- Fix out-of-bounds write in NFC activation handling (`919e0d7f1`, Kyle Hsiao)

## `system/core`
- ashmem_test: Add tests related to memfd's size file seals (`a5313eaec`, Isaac J. Manjarres)
- ashmem: Only handle size-sealed memfds (`1e5923617`, Isaac J. Manjarres)

## `vendor/crowdin`
- crowdin: Import translations (`0a7a9d8`, github-actions[bot])
- crowdin: Sync resources with upstream sources (`a6f6b36`, github-actions[bot])

## `vendor/lineage`
- release: Bump Security String to 2026-09-01 (`fe3293be`, Nolen Johnson)

# 07-Sep-2026

## `device/lineage/sepolicy`
- sepolicy: Add policy for SensitivePhoneNumbersService (`89d7484`, Nicholas Lim)

## `lineage/scripts`
- Merge https://github.com/LineageOS/scripts (`0404400`, hridaya)

## `vendor/crowdin`
- crowdin: Prepare translation infrastructure (`b8a7178`, Karan Parashar)
