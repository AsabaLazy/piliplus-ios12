# PiliPlus (iOS 12)

Auto-updating iOS 12.2–12.5.7 backport of PiliPlus built with zero upstream commit rollbacks.

English | [简体中文](README.zh-CN.md)

## Install

1. Download `PiliPlus_*_ios12_unsigned.ipa` from [Releases](https://github.com/AsabaLazy/piliplus-ios12/releases), or build from source via the GitHub Actions workflow.
2. On jailbroken iOS 12.2–12.5.7 devices, install `AppSync Unified` from Cydia or Sileo and install the IPA directly with Filza or `ideviceinstaller`.
3. On non-jailbroken devices, sign and install the IPA using Sideloadly, AltStore, or `zsign` with a personal Apple ID or developer certificate.

## Description

PiliPlus (iOS 12) packages the latest upstream [bggRGjQaUbCoE/PiliPlus](https://github.com/bggRGjQaUbCoE/PiliPlus) release for 64-bit iOS 12 devices (`iPhone 5s`, `iPhone 6 / 6 Plus`, `iPhone 6s / 6s Plus`, `iPad Air 1`, `iPad mini 2 / 3`, and `iPod touch 6`). It pairs a patched Flutter 3.47+ iOS 12 engine with `dyld2`-compatible `App.framework` relinking, `libmpv` / `FFmpeg` hardware-decoded playback, and runtime shims for iOS 13+ Metal, UIScene, and UIKit APIs.

Builds run automatically against upstream releases without reverting app features. File picking falls back to `UIDocumentPickerViewController` and `UIImagePickerController` on iOS 12, network reachability uses `SystemConfiguration`, and every IPA is verified offline against `iPhoneOS12.4.sdk` before publishing. See [AsabaLazy/oldcook](https://github.com/AsabaLazy/oldcook) for the build toolchain.

## Changelog

See the [Releases](https://github.com/AsabaLazy/piliplus-ios12/releases) page, or upstream [PiliPlus Releases](https://github.com/bggRGjQaUbCoE/PiliPlus/releases).

## Issues

Report iOS 12 crash logs and compatibility bugs in [Issues](https://github.com/AsabaLazy/piliplus-ios12/issues).

## FAQ

See [AsabaLazy/oldcook](https://github.com/AsabaLazy/oldcook/blob/main/Agent.md).
