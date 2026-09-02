# Slyvos Launcher Updates

Official development-build distribution repository for **Slyvos Launcher**.

Slyvos is a native Android launcher focused on **liquid minimalism, organic geometry, privacy, freedom, and a responsive user experience**.

> **Your device. Your data. Your choice.**

---

## What is this repository?

This repository is used to distribute **Slyvos Launcher development builds** to testers.

It contains:

* Development APKs
* Remote update manifests
* SHA-256 checksums
* Release notes
* Build metadata
* Minimum supported build information

The Slyvos Launcher can check this repository for newer builds and notify the tester when an update is available.

---

## Current Development Stage

**Pre-Alpha**

Slyvos is currently under active development.

Development builds are experimental and may contain:

* unfinished features
* UI changes
* bugs
* performance issues
* device compatibility issues

Builds are intended for testing and feedback rather than general public release.

---

## Build System

Slyvos uses development build numbers while the project is unfinished.

Example:

```text
Slyvos Pre-Alpha Build #002
```

The development build number is separate from Android's internal `versionCode`.

### Release stages

| Stage             | Meaning                                        |
| ----------------- | ---------------------------------------------- |
| Pre-Alpha         | Early development and core feature building    |
| Alpha             | Core functionality exists but remains unstable |
| Beta              | Feature set is mostly established              |
| Release Candidate | Final testing before release                   |
| v1.0              | First official finished release                |

The project will use **v1.0** only when the first official release is actually finished.

---

## Remote Updates

Slyvos uses a remote update system so testers do not need to connect their phones to the developer's computer for every new build.

The general update flow is:

```text
New Slyvos Build
       ↓
Build APK
       ↓
Publish APK
       ↓
Update Manifest
       ↓
Tester launches Slyvos
       ↓
Slyvos checks for updates
       ↓
New Build Detected
       ↓
Download APK
       ↓
Verify SHA-256
       ↓
Android Package Installer
       ↓
Updated Slyvos Build
```

Updates are installed through Android's normal package installation system. The launcher does **not** silently install updates.

---

## Update Manifest

The pre-alpha channel uses:

```text
pre-alpha.json
```

The manifest contains information such as:

```text
buildNumber
versionCode
versionName
releaseStage
releaseNotes
apkUrl
apkSha256
publishedAt
minimumSupportedBuildNumber
```

The SHA-256 checksum allows the launcher to verify that the downloaded APK matches the published build.

---

## Testing

If you are an approved Slyvos tester, please test the launcher on your real Android device and report anything unusual.

When reporting a bug, include:

* Slyvos build number
* Android version
* Device model
* What you were doing
* Steps to reproduce
* Expected behavior
* Actual behavior
* Screenshot or screen recording when useful

Good bug reports make debugging much faster.

---

## What Slyvos is Building

Slyvos is designed around a few principles:

**Privacy**
Your device should belong to you.

**Freedom**
The launcher should adapt to the user instead of forcing a single workflow.

**Minimalism**
Remove unnecessary visual and interaction noise.

**Fluidity**
Motion should communicate state and interaction, not exist purely for decoration.

**Organic Design**
Rounded, spatial, translucent surfaces form the visual language of Slyvos.

**Performance**
Visual polish should never come at the cost of a slow or frustrating experience.

**Community**
Slyvos is being developed with real users and testers involved throughout development.

---

## Repository Scope

This repository is specifically for **Slyvos Launcher development-build distribution**.

The launcher source code, development work, and other project resources are maintained separately.

This repository should remain focused on:

```text
APK Distribution
Update Metadata
Checksums
Release Information
```

---

## Current Build

**Slyvos Pre-Alpha Build #002**

Current development focus includes:

* Slyvos Home
* Dynamic Bar
* Dynamic Bar settings
* Remote update infrastructure
* Real-device testing

---

## License

Slyvos is currently under active development.

License information will be published when the project is ready for its public release.

---

<p align="center">
  <strong>slyvos</strong><br>
  building a calmer way to use Android.
</p>
