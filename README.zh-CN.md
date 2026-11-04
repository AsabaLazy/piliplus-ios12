# PiliPlus (iOS 12)

bggRGjQaUbCoE/PiliPlus 的 iOS 12.2–12.5.7 兼容构建版本。本项目使用 AI 辅助编码开发。

[English](README.md) | 简体中文

## 安装

1. 从 [Releases](https://github.com/AsabaLazy/piliplus-ios12/releases) 下载 `PiliPlus_*_ios12_unsigned.ipa`，或通过 GitHub Actions 从源码构建。
2. 已越狱的 iOS 12.2–12.5.7 设备，先在 Cydia 或 Sileo 中安装 AppSync Unified，再用 Filza 或 ideviceinstaller 安装。
3. 未越狱设备，使用 Sideloadly、AltStore 或 zsign 配合个人 Apple ID / 开发者证书签名后安装。

## 简介

PiliPlus (iOS 12) 面向 64 位 iOS 12 设备（iPhone 5s、iPhone 6 / 6 Plus、iPhone 6s / 6s Plus、iPad Air 1、iPad mini 2 / 3 及 iPod touch 6）构建 [bggRGjQaUbCoE/PiliPlus](https://github.com/bggRGjQaUbCoE/PiliPlus)。

## 兼容性

包含针对 iOS 12 编译的 Flutter 3.47+ 引擎、兼容 dyld2 的 App.framework 重链接、libmpv / FFmpeg 视频解码库，以及针对 iOS 13+ Metal、UIScene 与 UIKit 接口的 Objective-C 运行时垫片。

## 构建流程

通过 GitHub Actions 定时同步上游版本，底层构建与补丁工具链见 [AsabaLazy/oldcook](https://github.com/AsabaLazy/oldcook)。本项目使用 AI 辅助编码开发。

## 更新日志

见 [Releases](https://github.com/AsabaLazy/piliplus-ios12/releases) 页面，或上游 [PiliPlus Releases](https://github.com/bggRGjQaUbCoE/PiliPlus/releases)。

## 问题反馈

iOS 12 闪退日志与兼容性问题请在 [Issues](https://github.com/AsabaLazy/piliplus-ios12/issues) 中提交。
