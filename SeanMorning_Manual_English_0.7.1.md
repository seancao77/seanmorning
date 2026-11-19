# Sean Morning — Install Guide

> Version **v0.7.1** · updated 2026-11-19
> For Android 8.0+ and 64-bit (arm64) phones. Tested on: Samsung S25 Ultra (China, Android 16).
> This guide is updated with every release; in-app help is under ☰ → ❓ Help.

Sean Morning is your own personal AI companion, **running entirely on your phone**:

- No computer, no server needed;
- Your data (chats, memories, persona, API key) lives in an encrypted vault on the phone.

---

## 📚 Reading & analysis (new in 0.7.1)

- ☰ → 📚 **Reading & analysis**: let Morning pick books, list your own titles, or import your own e-books (EPUB / PDF / TXT / DOCX, up to 30 MB). After you confirm the list she reads in the background and writes a reading card for each book (also in 📄 Files). In the library you can ▶ listen to a 3-minute or 15-minute version, ask about the book, or generate a shareable piece.
- **Background reading** runs only while **charging on Wi-Fi** by default. For reliable background running, set Settings → Battery → Sean Morning to "**Unrestricted**" (same as the brief).
- It uses your own AI service and tokens: the page shows the estimated tokens, each plan has a budget and pauses when it's used up. Imported books stay in the phone's encrypted vault; only the relevant passages are sent to your chosen AI service. DRM-protected books cannot be opened.

---

## 1. What you need

| You need | Notes |
|---|---|
| Installer | `SeanMorning_android_<version>.apk` (~25 MB), plus a `.sha256` file for verification |
| Alibaba Bailian account | Used for chat, speech recognition, natural cloud voices, and web search — **one API key covers all of them**. New accounts include free quota; after that it's pay-as-you-go. Typical daily chatting costs a few yuan a month |
| Network | Any internet connection (Wi-Fi or mobile data) |

---

## 2. Install the app

1. Get the APK onto your phone (WeChat "File Transfer", USB cable, or a cloud drive).
2. Open the APK on the phone. If it says "install unknown apps", allow it for this one time (e.g. allow "My Files" or "WeChat" to install apps).
3. Tap **Install**, then **Open**.
4. (Optional) Verify: the value in the `.sha256` file should match `certutil -hashfile <file> SHA256` on a computer.

**Upgrading**: install the new version directly over the old one — chats, persona, and API key are kept. This requires the same signing key, which all official releases use.

**Do not uninstall first**: uninstalling also deletes the phone's vault.

---

## 3. First launch

1. The first time you tap **Voice** or **Talk**, it asks for the **microphone** permission — allow it.
2. The first time you use **Talk** mode, it asks for **notifications** — allow it. The call can continue after the screen locks thanks to that notification.
3. For the daily brief to be prepared on time: phone Settings → Apps → Sean Morning → Battery → **Unrestricted**.

---

## 4. Add your Alibaba Bailian API key (required)

1. **On the phone**, open <https://bailian.console.aliyun.com/cn-beijing/model/settings/api-key>, sign in with Alipay or an Alibaba Cloud account, and enable Bailian as prompted.
2. Tap **Create API Key** and copy it immediately. **The key is shown only once**, so create and copy it on the phone (no need to go through a computer).
3. Back in Sean Morning, open ☰ → 🧠 **AI models**.
4. In the **Fast replies (talk layer)** block:
   - Provider: **Alibaba Bailian**;
   - Model: `qwen3.7-plus` (smarter) or `qwen3.8-flash` (faster, cheaper);
   - Extra parameters: `{"enable_thinking":false}`;
   - Paste the key into the API key field, tap **Save**, then **Test**. A ✓ and first-word latency mean it works.
5. Do the same in **Complex tasks (work layer)**: model `qwen3.7-plus` (or `qwen3.8-max`). The key is already stored — no need to re-enter it.
6. When the balance runs out she tells you "balance insufficient" — top up in the Bailian console.

The key is stored only in the phone's encrypted vault; it's never shown on the page or sent anywhere else.

---

## 5. Voice, personality and background

- ☰ → 🎙️ **Voice**: engine **Cloud · Alibaba Bailian CosyVoice**, pick a voice you like, e.g. **龙应桃 Longyingtao (gentle & calm)** or **龙悦 Longyue (warm)**. You can set a monthly cap (default ¥20) and get a reminder at 80%. "Her volume" defaults to 90%. Choose "The phone's own (free)" if you don't want to spend.
- ☰ → 🎭 **Personality**: name her, choose the conversation mode, tune the style sliders, and pick **Language** — switch it to **English** here to turn the whole app English. Set her voice, then write or paste the personality profile; tap "Fill in the Morning V1.0 template" and adjust to taste. **Keep a copy of the profile text** so you can paste it back after switching phones.
- ☰ → 🎨 **Background**: pick a colour and shape, or tap "＋ Add photo/video" under "Your own backgrounds" to choose a photo or an MP4 video (up to 120 MB). Everything you add is saved; tap to switch, tap "Default" to go back, and only Delete removes it. Videos loop muted, and brightness is adjustable.
- ☰ → 🎨 **Digital persona** (0.6.2): under "Your own backgrounds", tap **Morning Modern** or **Morning Oriental**. She swaps to the matching video when idle, listening, and speaking; it loops muted and your choice persists. These are test videos that follow her state — not real-time lip sync.

---

## 6. Connections & brief

Open ☰ → 🔗 **Connections & brief**. The **Morning brief** is at the top; each connection is one row below. Tap a row to open its settings, and tap the pill on the right to switch it on or off. Changes save by themselves, or tap **Save** at the top.

| Connection | How to set it up |
|---|---|
| 🌅 Morning brief | Set a prepare time (default 06:45); you can add a few watch topics. Say "brief" to have it read aloud |
| ☀️ Weather | Just enter the city name, e.g. `Hangzhou`; the coordinates are looked up when you save |
| 📰 News | Tap recommended sources to add them in one tap (China News, IT Home, etc.); each source shows ✓ or ✗ |
| 📅 Phone calendar | Tap "Set up" to allow calendar access (also needed for adding events). Reads the phone calendar directly — no sign-up. Say "training class tomorrow 8am to 5pm, add to calendar" and a confirmation card appears; tap **Confirm** to add. Say "change to 8 to 5" or "delete this event" right after. For Outlook events: Samsung Calendar → Settings → Manage calendars → Add account → add your Outlook account |
| ⏰ Alarms & reminders | On by default, no permission needed — uses the phone's Clock app. Say "wake me at 6:30 tomorrow", "remind me in 10 minutes to turn off the stove"; right after, say "change to 7:30", "postpone 30 minutes", "cancel the alarm". Reminders more than a day away go into the phone calendar |
| 🎵 Music | Tap "Allow" so she can play your phone's songs; allow notification access so she can try to control QQ Music directly. Songs downloaded in QQ Music are encrypted and can only play inside QQ Music |
| 🔎 Web search | Uses the Bailian key above; turn it on and say "look up …" |
| 📧 Outlook calendar & mail | Optional; needs a free Microsoft app ID (Client ID) — a 36-character code with dashes, **not your mailbox**. The card has step-by-step instructions; details in [OUTLOOK.md](OUTLOOK.md). Personal accounts must register a free Azure account first (since 2024) before registering an app. Then tap "Sign in to Outlook" and follow the code on the page (to just see Outlook events, the "Phone calendar" above is simpler) |

**Share to Sean**: in WeChat, Toutiao, the browser, or your gallery, tap **Share** → **Send to Sean Morning**, and articles, links, and images go to her — one tap and she can summarise or fact-check them. The first time you may need to find Sean Morning under "More" in the share menu.

---

## 7. Switching phones & backup

- There's **no one-tap vault export yet** (planned). When switching phones, install the app on the new phone and redo steps 4–6. Paste the profile text you saved earlier.
- The vault key is protected by the phone's hardware (Android Keystore) and can't be copied to another phone, so the old phone's data can't be moved directly. This is by design, for security.

---

## 8. Troubleshooting

| Symptom | What to do |
|---|---|
| "No microphone permission" | Tap the button in the prompt to open permissions, or phone Settings → Apps → Sean Morning → Permissions → Microphone |
| Dictation does nothing / "balance insufficient" | Top up in the Bailian console; if it says "key needed", go back to step 4 |
| Music only opens QQ Music, or no sound | QQ Music doesn't let other apps control it. She'll switch to your phone's songs or radio; you can also allow notification access under Connections & brief → Music |
| Playback bar appears on its own / won't close | Tap ✕ (since 0.4.5 it always closes, and closed songs don't pop back). If you don't want the music feature, turn "Music" off in Connections & brief |
| Music silent / her voice too quiet | Press the side volume-up key: in the app that's the media volume, which changes her voice and music together. You can also set "Her volume" under ☰ → 🎙️ Voice (default 90%) |
| Words get cut off, or she answers slowly | Since 0.5.2 Voice starts recording immediately and waits for the last words; in Talk mode she answers 0.7 s after the sentence ends, longer mid-sentence. Adjust "How soon she answers" under ☰ → 🎙️ Voice → Talk |
| In Talk mode she takes her own words for yours | Since 0.5.4 she removes her own echo on the loudspeaker; just start talking to cut her off. If her voice gets quiet or music goes silent, turn off "Remove her own echo on the loudspeaker" under ☰ → 🎙️ Voice → Talk. Since 0.5.6 you can run "🔊 Loudspeaker echo test" on the same page, and copy "🩺 Call diagnostics" to the developer. Since 0.5.7 the test compares "Normal media mode" and "Call audio mode" and auto-picks the better one (or pick manually under "Echo cancelling on the loudspeaker"). In call audio mode the volume keys control the call volume |
| Cloud voice keeps dropping to the phone voice | Since 0.5.5 up to 2 sentences are synthesised at once and retried on failure; occasional failures only affect that sentence. If it still happens often, check the Bailian balance or try another voice under ☰ → 🎙️ Voice |
| Daily brief not ready on time | Set battery to "Unrestricted" (step 3) |
| How to use each feature | ☰ → ❓ Help |



