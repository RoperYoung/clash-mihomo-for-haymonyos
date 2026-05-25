# 纯血鸿蒙版 Clash Mihomo Harmony APK

面向 HarmonyOS 6.0 及以上设备的 Clash Meta for Android 改包名 APK 发布项目，内置 Clash 的 mihomo 内核，适合需要在鸿蒙系统环境中使用 mihomo 代理能力的用户。

本项目基于 [MetaCubeX/ClashMetaForAndroid](https://github.com/MetaCubeX/ClashMetaForAndroid/releases) 的发布版本进行包名调整。由于原项目 APK 在部分 HarmonyOS 设备上通过卓易通安装时会遇到无法安装或包名受限的问题，本项目提供改包名后的可安装版本。

> 当前仓库用于发布 APK、安装说明和校验信息。APK 建议挂载到 GitHub Releases，避免把大体积二进制文件直接提交进 Git 历史。

## 下载

请前往本项目的 [GitHub Releases](https://github.com/RoperYoung/clash-mihomo-for-haymonyos/releases) 页面下载最新版 APK：

- 下载最新的 APK 文件。
- 每个版本的具体文件名、版本号和校验值以对应 Release 页面为准。

## 核心特性

- 适配 HarmonyOS 6.0 及以上版本的 APK 安装与运行场景。
- 支持通过卓易通安装到鸿蒙设备。
- 内置 Clash 的 mihomo 内核，提供规则代理、订阅配置、DNS、TUN/VPN 等常见能力。
- APK 已签名，可直接下载安装。
- 包含多架构原生库，覆盖 `arm64-v8a`、`armeabi-v7a`、`x86` 和 `x86_64`。
- 跟随上游 ClashMetaForAndroid 版本持续更新。

## 来源与改包名说明

上游项目：[MetaCubeX/ClashMetaForAndroid](https://github.com/MetaCubeX/ClashMetaForAndroid/releases)

本项目不是 ClashMetaForAndroid 的官方上游仓库，而是面向 HarmonyOS + 卓易通安装场景的改包名发布版本。核心能力来自 Clash Meta for Android 与 Clash 的 mihomo 内核；本项目主要解决原包名在卓易通环境下无法安装或被限制的问题。

如果后续当前包名再次被系统、安装器或相关环境限制/ban，导致无法通过卓易通安装、更新或正常启动，请在 Issues 中反馈。提交 Issue 时建议附上设备型号、HarmonyOS 版本、卓易通版本、错误提示或截图，我会根据反馈继续更新包名并发布新版 APK。

## HarmonyOS 安装方式

1. 在 [GitHub Releases](https://github.com/RoperYoung/mihomo-clash-for-harmonyos/releases) 下载最新版 APK。
2. 打开卓易通，并选择安装本地 APK。
3. 按提示完成安装。
4. 首次启动时，根据系统提示授予 VPN、通知、网络访问等必要权限。
5. 导入你的 mihomo/Clash 订阅或本地配置文件后启用代理。

## 兼容说明

- 推荐系统：HarmonyOS 6.0 及以上。
- 推荐安装器：卓易通。
- Android SDK 信息：`minSdkVersion 21`，`targetSdkVersion 35`。
- 签名状态：APK Signature Scheme v1/v2 校验通过。
- 运行环境需要支持 APK 安装及 Android 兼容能力，实际体验可能受设备型号、系统版本和安装器版本影响。

## 项目定位

本项目目标是为 HarmonyOS 用户提供一个清晰、可校验、便于下载的 mihomo 内核 APK 发布入口，并在 HarmonyOS 操作系统上提供完整可用的 mihomo 使用体验。仓库本身不建议存放 APK 历史版本，历史版本应统一放在 GitHub Releases 中。

## 许可与声明

如果本项目要作为严格意义上的开源项目发布，建议同步公开对应源代码、构建脚本和许可证文件。当前仓库不把 APK 本身声明为仓库许可证覆盖范围；APK、mihomo 内核及 Clash 相关组件的版权和许可证以各自上游项目及 APK 实际包含内容为准。发布或再分发时，请确保遵守对应开源许可证和当地法律法规。
