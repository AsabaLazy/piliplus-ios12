# PiliPlus (iOS 12)

Auto-updating iOS 12.2–12.5.7 backport of PiliPlus built with zero upstream commit rollbacks.

English | [简体中文](README.zh-CN.md)

## Install

1. Download `PiliPlus_*_ios12_unsigned.ipa` from [Releases](https://github.com/AsabaLazy/piliplus-ios12/releases), or build from source via the GitHub Actions workflow.
2. On jailbroken iOS 12.2–12.5.7 devices, install AppSync Unified from Cydia or Sileo and install the IPA directly with Filza or ideviceinstaller.
3. On non-jailbroken devices, sign and install the IPA using Sideloadly, AltStore, or zsign with a personal Apple ID or developer certificate.

## Description

PiliPlus (iOS 12) ports [bggRGjQaUbCoE/PiliPlus](https://github.com/bggRGjQaUbCoE/PiliPlus) to 64-bit iOS 12 devices (iPhone 5s, iPhone 6 / 6 Plus, iPhone 6s / 6s Plus, iPad Air 1, iPad mini 2 / 3, and iPod touch 6).

## Compatibility

Includes a patched Flutter 3.47+ iOS 12 engine, dyld2-compatible App.framework relinking, libmpv / FFmpeg video decoding core, and runtime shims covering iOS 13+ Metal, UIScene, and UIKit APIs.

## Build Pipeline

Synced daily with upstream releases. See [AsabaLazy/oldcook](https://github.com/AsabaLazy/oldcook) for the underlying backport toolchain.

## Changelog

See the [Releases](https://github.com/AsabaLazy/piliplus-ios12/releases) page, or upstream [PiliPlus Releases](https://github.com/bggRGjQaUbCoE/PiliPlus/releases).

## Issues

Report iOS 12 crash logs and compatibility bugs in [Issues](https://github.com/AsabaLazy/piliplus-ios12/issues).
