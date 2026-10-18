# Neon Bastion 2: Android releases

Signed Android builds of **Neon Bastion 2**, the Unity remake of Neon Bastion. This repo only holds release files. The game's source is private.

- **Latest APK:** [Releases → latest](https://github.com/psteen-coder/neon-bastion-2-android/releases/latest). Each release is tagged `v<version>` and has `neon-bastion-2.apk` attached.
- **Update feed:** `https://raw.githubusercontent.com/psteen-coder/neon-bastion-2-android/dist/latest.json`. The game reads it on launch and offers newer builds. The `dist` branch holds `latest.json` and a copy of the current APK, which is the download fallback.
- **Package id:** `com.psteencoder.neonbastion2`. It installs alongside the original Neon Bastion and doesn't replace it.
- **Signing certificate:** `CN=Neon Bastion 2`, SHA-256 `dad37bc4c3ea7e6dbf5b32467a75b7748f451aa87c7b268d4eac423fddaf0c91`. Every release is signed with this key, so updates install over the previous version.

## Install (sideload)

1. On your Android phone, open the APK link from the latest release and download it.
2. When Android asks, allow your browser to install unknown apps.
3. Open the downloaded file and tap **Install**.

## How releases get here

Releases are published from FractalBox with `scripts/publish-android.ps1` in the private source repo. That script refuses to publish anywhere except this repo, and only APKs signed with the certificate above. This repo has no workflows, and GitHub Pages is off.
