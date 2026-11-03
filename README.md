# PiliPlus (iOS 12 Backport)

基于 [AsabaLazy/oldcook](https://github.com/AsabaLazy/oldcook) 向后移植工厂构建的 [bggRGjQaUbCoE/PiliPlus](https://github.com/bggRGjQaUbCoE/PiliPlus) **iOS 12.2 ~ 12.5.7** 自动追更版（零业务提交回退）。

## 支持设备与系统要求

- **系统版本**：iOS 12.2 及以上（推荐升级至该机型最高版本 **iOS 12.5.7** 或越狱常用版本 **iOS 12.4**，利用系统内置 ABI 稳定版 Swift 5 运行库）。
- **典型机型**：`iPhone 5s`、`iPhone 6 / 6 Plus`、`iPad Air (第 1 代)`、`iPad mini 2 / 3`、`iPod touch (第 6 代)` 以及所有更高版本 iOS 设备。

## 安装方式

Releases 页面提供的是经 `iPhoneOS12.4.sdk` 符号体检通过的无签名 `PiliPlus_*_ios12_unsigned.ipa`：

1. **已越狱设备（iOS 12.2 ~ 12.5.7）**：先在 Cydia / Sileo 安装 `AppSync Unified`，随后用 `Filza`、`ideviceinstaller -i` 或 `zsign -a` 直接安装。
2. **未越狱设备**：使用 `Sideloadly`、`AltStore` 或在 Linux/macOS 下使用 `zsign` 配合个人 Apple ID / 开发者证书签名后通过 `ideviceinstaller` 安装。

## 自动化追更机制

- 每日定时巡检上游 `bggRGjQaUbCoE/PiliPlus` 最新 Release，自动拉取 `AsabaLazy/oldcook` 预编译的 iOS 12 版 `Flutter.xcframework` 与插件垫片构建 `.ipa`。
- 每次打包均经过离线 Mach-O 与 `iPhoneOS12.4.sdk` 符号守门校验（`Verdict: PASS` 才自动发版，出现新增不兼容符号则自动拦截并创建诊断 Issue）。
