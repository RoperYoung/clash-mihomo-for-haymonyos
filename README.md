# Mihomo Harmony APK

面向 HarmonyOS 6.0 及以上设备的 Clash Meta for Android APK 发布项目，内置 Clash 的 mihomo 内核，适合需要在鸿蒙系统环境中使用 mihomo 代理能力的用户。

> 当前仓库用于发布 APK、安装说明和校验信息。APK 建议挂载到 GitHub Releases，避免把大体积二进制文件直接提交进 Git 历史。

## 核心特性

- 适配 HarmonyOS 6.0 及以上版本的 APK 安装与运行场景。
- 支持通过卓易通（Zotong）安装到鸿蒙设备。
- 内置 Clash 的 mihomo 内核，提供规则代理、订阅配置、DNS、TUN/VPN 等常见能力。
- APK 已签名，可直接下载安装。
- 包含多架构原生库，覆盖 `arm64-v8a`、`armeabi-v7a`、`x86` 和 `x86_64`。

## 下载

请前往本项目的 GitHub Releases 页面下载最新版 APK：

- 文件名：`clash-meta-neohub-mate-zhuoyitong.apk`
- 当前版本：`2.11.27.Meta`
- 包名：`com.neohub.clash.mate`
- 文件大小：约 `75 MB`
- SHA-256：`64407f0415d30a9e7c6e072032581ec60843655c22fca4fd8f32eda2e25612a0`

下载后可使用下面的命令校验文件完整性：

```bash
shasum -a 256 clash-meta-neohub-mate-zhuoyitong.apk
```

输出应与上方 SHA-256 值一致。

## HarmonyOS 安装方式

1. 在 GitHub Releases 下载 `clash-meta-neohub-mate-zhuoyitong.apk`。
2. 打开卓易通（Zotong），并选择安装本地 APK。
3. 按提示完成安装。
4. 首次启动时，根据系统提示授予 VPN、通知、网络访问等必要权限。
5. 导入你的 mihomo/Clash 订阅或本地配置文件后启用代理。

## 兼容说明

- 推荐系统：HarmonyOS 6.0 及以上。
- 推荐安装器：卓易通（Zotong）。
- Android SDK 信息：`minSdkVersion 21`，`targetSdkVersion 35`。
- 签名状态：APK Signature Scheme v1/v2 校验通过。
- 运行环境需要支持 APK 安装及 Android 兼容能力，实际体验可能受设备型号、系统版本和安装器版本影响。

## 项目定位

本项目目标是为 HarmonyOS 用户提供一个清晰、可校验、便于下载的 mihomo 内核 APK 发布入口，并在 HarmonyOS 操作系统上提供完整可用的 mihomo 使用体验。仓库本身不建议存放 APK 历史版本，历史版本应统一放在 GitHub Releases 中。

## 许可与声明

如果本项目要作为严格意义上的开源项目发布，建议同步公开对应源代码、构建脚本和许可证文件。当前仓库不把 APK 本身声明为仓库许可证覆盖范围；APK、mihomo 内核及 Clash 相关组件的版权和许可证以各自上游项目及 APK 实际包含内容为准。发布或再分发时，请确保遵守对应开源许可证和当地法律法规。
