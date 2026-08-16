<div align="center">

# 🔓 Threads Android SSL Pinning Bypass

**Decrypt and inspect Threads' full HTTPS traffic on a stock, non-rooted Android device — 2026 working build.**

[![Download APK](https://img.shields.io/badge/⬇_Download_APK_(v442.0.0)-000000?style=for-the-badge&logo=threads&logoColor=white)](../../releases/latest)
[![Telegram](https://img.shields.io/badge/Telegram-26A5E4?style=for-the-badge&logo=telegram&logoColor=white)](https://t.me/MUH4MM4DSH4KIB)

![Android](https://img.shields.io/badge/Android_10--14+-3DDC84?style=flat-square&logo=android&logoColor=white)
![ARM64](https://img.shields.io/badge/arm64--v8a-blue?style=flat-square)
![Version](https://img.shields.io/badge/Threads-v442.0.0.46.79-000000?style=flat-square&logo=threads&logoColor=white)
![Root](https://img.shields.io/badge/Root-Not_Required-brightgreen?style=flat-square)

🔓 Pinning defeated&nbsp;&nbsp;·&nbsp;&nbsp;🔐 Login capture&nbsp;&nbsp;·&nbsp;&nbsp;📰 Feed & posts&nbsp;&nbsp;·&nbsp;&nbsp;📱 No root

<img width="578" height="1280" alt="Threads Android SSL Pinning Bypass PoC – Traffic Captured" src="https://github.com/user-attachments/assets/1927e854-3f30-4ece-af5f-f4c0042777d9" />

</div>

> [!TIP]
> **Download the patched APK** from the **[Releases](../../releases/latest)** section — or message me on **[Telegram](https://t.me/MUH4MM4DSH4KIB)** for the newest build or another version.

---

## 📦 Build

| App | Package | Version | ABI |
|:----|:--------|:-------:|:---:|
| **Threads for Android** | `com.instagram.barcelona` | `442.0.0.46.79` | `arm64-v8a` |

---

## 🎯 What You Can Capture

| Surface | Exposed in cleartext |
|:--------|:---------------------|
| 🔐 **Login via Instagram** | auth token exchange and session handling |
| 📰 **Feed & timeline** | for-you / following ranking and GraphQL queries |
| ✍️ **Posts & replies** | create, like, repost, and quote endpoints |
| 👤 **Profile & follows** | profile data and follow-graph requests |
| 🖼️ **Media** | image/video upload and CDN delivery |
| 📊 **Telemetry** | device telemetry and A/B assignments |

---

## ⚙️ Requirements

**Android 10–14+** on an ARM device (`arm64-v8a` — virtually all modern phones), plus a MITM proxy — Burp Suite, mitmproxy, Reqable, or Proxypin.

> [!NOTE]
> **No root required** — install the patched APK and go (rooted devices work too). On emulators (Nox / LDPlayer / MEmu / BlueStacks), enable **ARM translation** — this build ships `arm64` native libraries, so x86/x86_64 emulators need the translation layer.

---

## 🚀 Setup

1. **Uninstall** the official Threads app *(signatures conflict)*.
2. **Download** the patched APK from [Releases](../../releases/latest) and **install** it on your device or emulator.
3. **Trust your proxy CA** — **Settings → Security → Encryption & credentials → Install a certificate → CA certificate**.
4. **Set the Wi-Fi proxy** — **Settings → Wi-Fi → (network) → Proxy → Manual** → your PC's IP and port.
5. **Launch Threads** — decrypted HTTPS streams into your proxy in real time.

> [!WARNING]
> If traffic doesn't appear immediately, **force-stop and relaunch** the app.

---

<div align="center">

## 💼 Need a Custom Bypass?

**Custom SSL pinning bypass · automated patching scripts · full reverse-engineering projects** — any Android or iOS app.

[![Request Custom Work](https://img.shields.io/badge/Message_me_on_Telegram-26A5E4?style=for-the-badge&logo=telegram&logoColor=white)](https://t.me/MUH4MM4DSH4KIB)

</div>

---

> [!NOTE]
> **Disclaimer** — For educational and security-research purposes only. Not affiliated with, endorsed by, or connected to Meta, Threads, or Instagram. All trademarks belong to their respective owners. Only analyze traffic on accounts and devices you own or are authorized to test. Provided "as is", without warranty of any kind.

---

## 🔗 Related Projects

| App | Platform | Repository |
|-----|----------|------------|
| Threads | iOS | [Threads iOS SSL Pinning Bypass](https://github.com/0xSHAK1B/Threads-iOS-SSL-Pinning-Bypass) |
| Instagram | Android | [Instagram SSL Pinning Bypass](https://github.com/0xSHAK1B/Instagram-SSL-Pinning-Bypass) |
| Edits | Android | [Edits SSL Pinning Bypass](https://github.com/0xSHAK1B/Edits-SSL-Pinning-Bypass) |
| Instants | Android | [Instants SSL Pinning Bypass](https://github.com/0xSHAK1B/Instants-SSL-Pinning-Bypass) |
| Facebook | Android | [Facebook SSL Pinning Bypass](https://github.com/0xSHAK1B/Facebook-SSL-Pinning-Bypass) |
| TikTok | Android | [TikTok SSL Pinning Bypass](https://github.com/0xSHAK1B/TIKTOK-SSL-Pinning-Bypass) |

---

<div align="center">

### 💖 Support This Project

Please **⭐ star the repo** — it helps others find it and keeps the builds coming.

| Currency | Address |
|:---------|:--------|
| **BTC / ETH** | `0xea9a566a5123c3a1b8d60f8bdd845835716668f0` |
| **USDT (TRC-20)** | `THssAZhUQEEsw15211rAaRLGRjSWXMX4PW` |

[![Telegram](https://img.shields.io/badge/@MUH4MM4DSH4KIB-26A5E4?style=for-the-badge&logo=telegram&logoColor=white)](https://t.me/MUH4MM4DSH4KIB)

</div>
