# Sean Morning · 个人 AI 伙伴

一个以**语音为主、以手机为主**的个人 AI 伴侣。整个 App 就运行在你的手机上，不需要电脑、不需要服务器；聊天、记忆、人格设定和 API Key 都加密保存在手机里。

## 下载

推荐从「发行版」页下载（有版本号和直接下载按钮）：
<https://github.com/seancao77/seanmorning/releases>

| 版本 | 直接下载 | 适合谁 |
|---|---|---|
| 普通版 | [SeanMorning_android_0.7.3.apk](https://github.com/seancao77/seanmorning/releases/download/v0.7.3/SeanMorning_android_0.7.3.apk) | 想用自己的 AI 账号的朋友 |
| 家庭版 | [SeanMorning_family_android_0.7.3.apk](https://github.com/seancao77/seanmorning/releases/download/v0.7.3/SeanMorning_family_android_0.7.3.apk) | 家人 / 亲友（已预配好） |

> 国内用户也可以到 gitee 镜像仓库下载：<https://gitee.com/magnificent-masterpiece/seanmorning/releases>

## 0.7.3 新增：🌐 读书分享 → 发布到自己的网站

☰ → 📚 阅读与分析：让 Morning 帮你挑书（比如说「帮我挑 10 本关于沟通的书」）、自己列书名，或导入自己的电子书（EPUB / PDF / TXT / DOCX）。确认书单后她在后台读（默认只在充电 + Wi-Fi 时），每本生成读书卡；书房里可以听 3 分钟 / 15 分钟讲书、问这本书、生成分享稿。

**0.7.2 新增「🌐 分享包」**（默认关闭）：把读完的书做成分享包——读书卡公开部分 + 讲书音频，🔒 私人内容、导入原文、联系方式都会去掉，页面标明由 AI 整理朗读；可导出成手机上的 HTML 文件。

**0.7.3 新增「🌐 发布到自己的网站」**：可以把读书分享发布到你自己的网站（需满足一定要求）。普通版和家庭版都有。

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

## Sean Morning · Personal AI Companion

A voice-first, phone-first personal AI companion. The whole app runs on your phone — no computer, no server. Chats, memories, persona and API key are encrypted in a vault on the phone.

### Download

Recommended: download from the Releases page (with version numbers and direct download buttons):
<https://github.com/seancao77/seanmorning/releases>

| Edition | Direct download | For whom |
|---|---|---|
| Standard | [SeanMorning_android_0.7.3.apk](https://github.com/seancao77/seanmorning/releases/download/v0.7.3/SeanMorning_android_0.7.3.apk) | Friends who want to use their own AI account |
| Family | [SeanMorning_family_android_0.7.3.apk](https://github.com/seancao77/seanmorning/releases/download/v0.7.3/SeanMorning_family_android_0.7.3.apk) | Family / friends (pre-configured) |

> Users in China can also download from the gitee mirror: <https://gitee.com/magnificent-masterpiece/seanmorning/releases>

### New in 0.7.3: 🌐 Reading share → publish to your own site

☰ → 📚 Reading & analysis: let Morning pick books (say "pick 10 books on communication"), list your own titles, or import your own e-books (EPUB / PDF / TXT / DOCX). After you confirm the list she reads in the background (by default only while charging on Wi-Fi) and writes a reading card for each book. In the library you can listen to a 3- or 15-minute version, ask about the book, or generate a shareable piece.

**New in 0.7.2 — "🌐 share package"** (off by default): turn a finished book into a share package — the public part of the reading card plus the narration audio; 🔒 private content, imported source text and contact details are stripped, and the page is marked as AI-read. You can export it as an HTML file on the phone.

**New in 0.7.3 — "🌐 publish to your own site"**: you can publish your reading shares to your own website (subject to certain requirements). Both Standard and Family editions include it.

### The two editions

- **Standard**: install, choose your own AI service, and enter your own API key.
- **Family**: model, voice, weather, news and the brief are pre-configured; on first launch, paste the API key the sharer gives you.

### Install

1. Get the APK onto your phone (WeChat "File Transfer", USB cable, or a cloud drive).
2. Open the APK and allow "install unknown apps" when asked.
3. Open the app and follow the install guide.

See the install guide: an HTML version (opens right in the phone browser) and a Markdown version are attached to the release — HTML is recommended.

### Requirements

- Android 8.0+
- 64-bit (arm64) phone

### You'll need

- An **Alibaba Bailian (DashScope)** account: one API key covers chat, speech recognition, natural cloud voices and web search. New accounts include free quota.

### Privacy & security

- Everything runs on the phone; your data never leaves the device.
- Chats, memories, persona and API key are stored in an encrypted vault (AES-256-GCM), protected by the phone's hardware (Android Keystore).

### Upgrading

New versions are released on the Releases page. Install the latest APK over the old one — all data is kept. **Do not uninstall first** (uninstalling deletes the vault).

---

© 2026 Sean Morning
