# Threads SSL Pinning Bypass 2026 – Intercept HTTPS Traffic on Android (Root & No Root)

[![Telegram](https://img.shields.io/badge/💬_Chat_on_Telegram-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white&labelColor=121212&color=26A5E4&logoWidth=20)](https://t.me/MUH4MM4DSH4KIB)
![Android](https://img.shields.io/badge/Android-3DDC84?style=for-the-badge&logo=android&logoColor=white)
![ARM64](https://img.shields.io/badge/ARM64--v8a-Supported-blue?style=for-the-badge)
![x86_64](https://img.shields.io/badge/x86__64-Supported-blue?style=for-the-badge)

> **Bypass SSL certificate pinning in Meta Threads on Android** to intercept, capture, and analyze HTTPS network traffic using proxy tools like Burp Suite, mitmproxy, Reqable, or Proxypin — works on both **rooted** and **non-rooted** devices in 2026.

---

## Overview of this project

Meta's **Threads** app enforces **SSL/TLS certificate pinning** to prevent third-party proxy tools from intercepting its HTTPS traffic. This repository provides a **pre-patched Threads APK** with certificate pinning disabled, enabling security researchers, penetration testers, and developers to capture and inspect Threads network requests and API responses.

---

## Proof of Concept

<img width="720" height="1640" alt="Image" src="https://github.com/user-attachments/assets/23f94cd3-657b-4770-a960-866cb1645990" />



▶️ [**Watch the Full Video Demonstration**](https://github.com/user-attachments/assets/259410ce-2f80-4b2a-82af-361e42e56ffe)

---

## Supported Threads Version

| App | Version | Architecture | Status |
|-----|---------|--------------|--------|
| Threads | **427.0.0.48.72** | `arm64-v8a` | ✅ Bypassed |
| Threads | **427.0.0.48.72** | `x86_64` | ✅ Bypassed |

> Need a **newer version**? [Contact me on Telegram](https://t.me/MUH4MM4DSH4KIB) for the latest bypassed build.

---

## Requirements

### Option A: Physical Android Device (No Root Required)

- Android phone or tablet running **Android 7.0+**
- MITM proxy tool installed on the same device or on your local network:
  - [**Reqable**](https://reqable.com) — modern, feature-rich HTTP/HTTPS debugging proxy
  - [**Proxypin**](https://proxypin.com) — free and lightweight traffic capture tool

### Option B: Android Emulator on PC

- Windows, macOS, or Linux PC with an Android emulator:
  - [**Nox Player**](https://www.bignox.com/) — popular Android emulator for Windows/Mac
  - [**LDPlayer**](https://www.ldplayer.net/) — fast Android emulator optimized for performance
- Desktop MITM proxy tool:
  - [**Burp Suite**](https://portswigger.net/burp) — industry-standard web security testing proxy
  - [**mitmproxy**](https://mitmproxy.org/) — open-source interactive HTTPS proxy
  - [**Reqable**](https://reqable.com) — cross-platform HTTP debugging proxy
  - [**Proxypin**](https://proxypin.com) — lightweight proxy with mobile support

---

## How to Bypass Threads SSL Pinning (Step-by-Step)

### Step 1: Download the Patched APK

Download the SSL pinning bypassed Threads APK from this repository's [Releases](../../releases) section. Choose the correct architecture for your device:
- **`arm64-v8a`** — Most modern Android phones and tablets
- **`x86_64`** — Android emulators (Nox Player, LDPlayer, etc.)

### Step 2: Install the Patched Threads APK

- **Uninstall** the official Threads app if already installed (signatures will conflict)
- **Enable** "Install from Unknown Sources" in your Android settings
- **Install** the downloaded patched APK

### Step 3: Set Up Your Proxy Tool

1. Open your proxy tool (Burp Suite, mitmproxy, Reqable, or Proxypin)
2. **Export** the proxy's CA certificate
3. **Install and trust** the CA certificate on your Android device:
   - Go to **Settings → Security → Install certificates from storage**
   - On Android 11+, you may need to move the cert to the system trust store (root required) or use your proxy tool's built-in certificate installer
4. **Configure** your device's Wi-Fi proxy settings to point to the proxy

### Step 4: Capture Threads HTTPS Traffic

1. Launch the patched **Threads** app
2. Browse, post, or interact normally
3. Watch **decrypted HTTPS requests and responses** appear in your proxy tool in real time


---

## Related Projects

- [**Instagram SSL Pinning Bypass**](https://github.com/MUH4MM4D-SH4KIB) — Intercept Instagram HTTPS traffic on Android
- [**Facebook SSL Pinning Bypass**](https://github.com/MUH4MM4D-SH4KIB) — Capture Facebook API requests and responses
- [**TikTok SSL Pinning Bypass**](https://github.com/MUH4MM4D-SH4KIB) — Bypass TikTok certificate pinning for traffic analysis
- [**Snapchat SSL Pinning Bypass**](https://github.com/MUH4MM4D-SH4KIB) — Decrypt Snapchat HTTPS traffic on Android

---

## Contact & Latest Builds

For the **most up-to-date** SSL pinning bypassed Threads APK and support:

[![Telegram](https://img.shields.io/badge/💬_Chat_on_Telegram-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white&labelColor=121212&color=26A5E4&logoWidth=20)](https://t.me/MUH4MM4DSH4KIB)
