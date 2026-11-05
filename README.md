# KAC Duty Officer's Desk — Public Releases

This repository is the public download point for **KAC Duty Officer's Desk**, the
Karachi Aero Club's local-first application for pilot-licensing documentation,
flight-check records, application tracking and CAA form packs.

The application source code is maintained in a private repository. Nothing in
this repository is application source code, and no applicant data is published
here.

## Download

Open the [latest release](https://github.com/uzair-suria/kac-duty-officers-desk-releases/releases/latest)
and choose the file for your platform:

| Platform | File | Notes |
| --- | --- | --- |
| Windows x64 | `KAC.Duty.Officers.Desk_<version>_x64-setup.exe` | NSIS installer. Unsigned, so SmartScreen may warn. |
| macOS Apple Silicon | `KAC.Duty.Officers.Desk_<version>_aarch64.dmg` | Unsigned unless Apple signing was configured. |
| macOS Intel | `KAC.Duty.Officers.Desk_<version>_x64.dmg` | Unsigned unless Apple signing was configured. |
| macOS `.app` bundles | `KAC.Duty.Officers.Desk_apple-silicon.app.zip`, `KAC.Duty.Officers.Desk_intel.app.zip` | Zipped application bundles for manual installation. |
| Android | `app-universal-debug.apk` | Debug APK for evaluation; not a Play Store build. |
| iOS Simulator | `ios-simulator.app.zip` | Simulator-only build. It is **not** an installable iPhone/iPad, TestFlight or App Store build. |

## Important

- Builds are unsigned unless signing credentials were supplied to the build.
- On macOS, right-click the app and choose **Open** the first time.
- Android and iOS builds do not include the desktop Python document-enhancement
  sidecar.
- Generated forms and document packs are drafts. Staff must review current CAA
  requirements and complete signatures, stamps and approvals manually.
- Applicant data stays on the user's device. It is never uploaded here.

## How releases are produced

The private source repository builds Windows, macOS, Android and iOS artifacts
with GitHub Actions. Its **Publish release** workflow creates the private
release and mirrors the same tag, notes and assets to this repository. Do not
upload files here manually; the workflow is the source of truth.
