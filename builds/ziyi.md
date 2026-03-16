# Evolution X – Android 16 QPR2 Update

**Android version:** 16 QPR2  
**Security patch:** March 2026

---

## 📌 Notes
- Install a **HyperOS 2 firmware** according to your region  
  https://xmfirmwareupdater.com/firmware/ziyi
- LineageOS-based source
- **Signed build**
- Always dirty flash **at your own risk**.  
  If your device bootloops, revert to a previous working build.
- **KernelSU 3.1 + SUSFS 2.0**
- Includes:
  - MiuiCamera
  - Dolby Atmos
  - eSIM support

---

## 📱 Device Changes

- **parts:** Remove unused Doze implementation and service  
- **sensors:** Use stack allocation for `_oem_msg` to avoid memory leaks

---

## ⚙️ Notable ROM Changes

### SystemUI
- Do not collapse panel when interacting with seekbar
- Reduce unnecessary invalidation of ongoing chip background color
- Fix ringer tile rendering for vibrator support and DND state
- Improve music chip popup UI
- Periodically re-evaluate sessions to catch stale playback
- Refactor album art, icon, and playback handling
- Smoother seekbar in ongoing chip popup UI
- Update chip max width

### Settings
- Hide Ambient display from search
- Location:
  - Move mock location app picker to Location settings
  - Grey out mock override toggle until an app is selected

### Framework / Audio
- Skip updating value-added A2DP offload codecs to MM audio over AIDL
- `fixup! audio:` Allow opting out of `speaker_layout_channel_mask` field

### Misc
- **ColumbusService:** Improve Vietnamese translations
- **Evolver:** Update team members
