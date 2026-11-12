# Sean Morning · 个人 AI 伙伴

一个以**语音为主、以手机为主**的个人 AI 伴侣。整个 App 就运行在你的手机上，不需要电脑、不需要服务器；聊天、记忆、人格设定和 API Key 都加密保存在手机里。

## 下载

推荐从「发行版」页下载（有版本号和直接下载按钮）：
<https://gitee.com/magnificent-masterpiece/seanmorning/releases>

| 版本 | 直接下载 | 适合谁 |
|---|---|---|
| 普通版 | [SeanMorning_android_0.6.8.apk](https://gitee.com/magnificent-masterpiece/seanmorning/releases/download/v0.6.8/SeanMorning_android_0.6.8.apk) | 想用自己的 AI 账号的朋友 |
| 家庭版 | [SeanMorning_family_android_0.6.8.apk](https://gitee.com/magnificent-masterpiece/seanmorning/releases/download/v0.6.8/SeanMorning_family_android_0.6.8.apk) | 家人 / 亲友（已预配好） |

> 每个 APK 都有同名的 `.sha256` 文件（在仓库文件列表里），用于校验下载是否完整（可选）。

> **下载提示**：如果下载下来的 APK 文件名带了 `.zip` 后缀（例如 `xxx.apk.zip`），把 `.zip` 去掉、重命名回 `.apk` 再安装即可——文件内容没变，只是 gitee 误判了文件类型。

## 两个版本的区别

- **普通版**：安装后自己选 AI 服务、填自己的 API Key。
- **家庭版**：模型、声音、天气、新闻、早报都已预先配好；安装后第一次打开会弹一个框，**粘贴分享者给你的 API Key** 即可直接使用。

## 安装

1. 把 APK 传到手机（微信「文件传输助手」、USB 数据线、网盘都可以）。
2. 在手机上点开 APK，按提示允许「安装未知应用」并安装。
3. 打开 App，按《安装手册》完成配置。

完整说明见《安装手册》：发行版里有 **HTML 版**（手机浏览器直接打开）和 Markdown 版，推荐下载 HTML 版。

## 系统要求

- Android 8.0 及以上
- 64 位（arm64）手机

## 需要准备

- **阿里百炼（DashScope）账号**：聊天、语音识别、云端自然声音、联网搜索都用一个 API Key。新账号有免费额度。

## 隐私与安全

- 全部在手机上运行，数据不离开你的设备。
- 聊天、记忆、人格设定、API Key 都保存在手机加密保险箱（AES-256-GCM），密钥由手机硬件（Android Keystore）保护。

## 升级

新版本会继续以「发行版」形式发布。下载最新 APK 直接覆盖安装即可，数据全部保留；**不要先卸载再装**（卸载会清掉手机里的保险箱）。

---

© 2026 Sean Morning
