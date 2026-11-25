<div align="center">

# Steamify Live

**Stream to Twitch, YouTube and Kick at the same time — with 0% extra GPU.**

The all-in-one ecosystem for OBS Studio creators: simultaneous multistreaming, unified chat, a real-time events center, game presets with an audience thermometer, and encrypted cloud backup — 100% free.

[![Latest release](https://img.shields.io/github/v/release/fjefferson/steamify-live-releases?style=for-the-badge&label=latest&color=9146FF)](https://github.com/fjefferson/steamify-live-releases/releases/latest)
[![Downloads](https://img.shields.io/github/downloads/fjefferson/steamify-live-releases/total?style=for-the-badge&color=2ea44f)](https://github.com/fjefferson/steamify-live-releases/releases)
[![Release date](https://img.shields.io/github/release-date/fjefferson/steamify-live-releases?style=for-the-badge&color=blue)](https://github.com/fjefferson/steamify-live-releases/releases/latest)

![OBS Studio](https://img.shields.io/badge/OBS%20Studio-30%20%7C%2031%20%7C%2032%20%7C%2033%2B-302E31?style=flat-square&logo=obsstudio&logoColor=white)
![Platform](https://img.shields.io/badge/Windows-10%20%7C%2011%20(64--bit)-0078D4?style=flat-square&logo=windows&logoColor=white)
![C++20](https://img.shields.io/badge/C%2B%2B-20-00599C?style=flat-square&logo=cplusplus&logoColor=white)
![Price](https://img.shields.io/badge/price-free-brightgreen?style=flat-square)
![No watermark](https://img.shields.io/badge/watermark-none-success?style=flat-square)
![Languages](https://img.shields.io/badge/UI-English%20%7C%20Portugu%C3%AAs%20(BR)-orange?style=flat-square)

[![Twitch](https://img.shields.io/badge/Twitch-9146FF?style=flat-square&logo=twitch&logoColor=white)](https://www.twitch.tv)
[![YouTube](https://img.shields.io/badge/YouTube-FF0000?style=flat-square&logo=youtube&logoColor=white)](https://www.youtube.com)
[![Kick](https://img.shields.io/badge/Kick-53FC18?style=flat-square&logo=kick&logoColor=black)](https://kick.com)

[**Website**](https://live.steamify.com.br) · [**Download**](https://github.com/fjefferson/steamify-live-releases/releases/latest) · [**All releases**](https://github.com/fjefferson/steamify-live-releases/releases) · [**Support the project**](https://livepix.gg/jeffnaplay)

</div>

---

## Why Steamify Live?

| | |
|---|---|
| ⚡ **0% extra GPU** | Reuses the frames from your existing hardware encoder (NVENC, AMF, QSV, x264) — no duplicated rendering. |
| 💸 **$0 / month** | No cloud-server subscription. Everything runs locally inside your OBS. |
| ⏱️ **0 s extra delay** | Direct RTMP connection to each platform, so your viewers get your signal in real time. |
| 🔒 **100% private** | Your video and stream keys never pass through third-party servers. |

## Features

### 📡 Multistreaming with zero GPU impact
Stream to Twitch, YouTube, Kick, TikTok, Facebook or any custom RTMP server simultaneously. The plugin clones the already-encoded output (*Hardware Passthrough*) instead of re-rendering your scene.

### 🎉 Unified Events Center — *"Steamify Live — Events"* dock
Follow and thank your whole community from a single native OBS dock.
- Follows, Subs / Resubs / Gift Subs, Raids, Bits, Super Chats, Super Stickers and new Members from Twitch, Kick and YouTube.
- One-click **"Seen"** button, so you never leave a subscriber or donor unanswered.
- Filters: *All*, *Subs & Members*, *Donations & Bits*, *Followers*, *Hide seen*.
- Persistent local history, plus an event simulator (tagged `SIMULATED`) with selective cleanup that never touches real events.

### 💬 Unified cross-platform chat
Read and reply to Twitch, Kick and YouTube messages in one clean window — with badges (Mod, VIP, Sub, Crown), subscriber emotes, platform selection for replies and a native C++ anti-spam filter for very busy chats.

### 🎮 Smart presets & audience thermometer
Switch title and game with one click (Twitch Helix, Kick v2 and YouTube Studio) and check the demand for a game before you go live:
- **Twitch & Kick:** live viewers and followers for the category.
- **YouTube Gaming:** live viewers in the category (cached locally, no API quota spent).

### 👥 Adaptive audience dock
See the exact sum of simultaneous viewers across all platforms, combined or per platform. The glassmorphism panel adapts to narrow vertical or wide horizontal docks and works with any OBS theme.

### ☁️ Steamify Cloud — encrypted backup & restore
Back up your RTMP destinations, keys, tokens, presets and profile picture with **zero-knowledge AES-256-GCM** encryption. Tied to your Twitch identity, with an optional 4–6 digit security PIN. Reformatting your PC? Restore everything in about 2 seconds.

### 📱 Vertical canvas ready
Compatible with the Aitum Vertical plugin for TikTok, Shorts and Reels streams, with a built-in safeguard against accidentally going public while in Twitch's bandwidth-test mode.

### 🎙️ Local AI captions
On-device speech-to-text captions powered by [whisper.cpp](https://github.com/ggml-org/whisper.cpp).

## Steamify Cam *(optional companion plugin)*

The installer can also include **Steamify Cam**, a webcam studio for OBS:
- **Google Meet Beauty** — skin smoothing, studio lighting and natural detail.
- **Instagram-style presets** — Natural Glow, Golden Hour, Cinema, Cyber Neon and more.
- **150+ 3D `.cube` LUTs** — Portrait, Cinema, Color Boost and more (optional extra pack).
- **AI filter generator** — creates filters from text using your Steamify Live AI key.
- **GPU-friendly** — real-time performance meter right inside OBS.

## Installation

1. **Download** `Steamify-Live-Installer-vX.Y.Z.exe` from the [latest release](https://github.com/fjefferson/steamify-live-releases/releases/latest).
2. **Run the installer.** It detects your OBS Studio folder automatically (you can change it) and lets you choose between *Steamify Live only* or *Full installation* (Steamify Live + Steamify Cam). Close OBS first.
3. **Open OBS Studio** and go to **Docks → Steamify Live**. Start streaming to the world!

To update, just run the newer installer over your current installation. To remove it, use *Apps → Installed apps* in Windows.

### Requirements

- Windows 10 or 11 (64-bit)
- OBS Studio 30, 31, 32 or 33+
- Upload bandwidth equal to the sum of your active destinations (e.g. 6,000 Kbps on Twitch + 6,000 Kbps on YouTube = 12,000 Kbps)

## Verifying your download

Every release lists the **SHA256** checksum of the installer in its notes. To check it on Windows:

```powershell
Get-FileHash .\Steamify-Live-Installer-vX.Y.Z.exe -Algorithm SHA256
```

The result must match the value published in the release notes.

## How it compares

| Feature | **Steamify Live** (native) | Restream.io (cloud) | Typical OBS plugin |
|---|---|---|---|
| Monthly cost | **Free** | $19–$49 / month | Free |
| Extra GPU usage | **0%** (hardware clone) | 0% (single upload) | 0% |
| Extra latency | **0 s** | +3 to +6 s | 0 s |
| Game presets + audience thermometer | **Yes** | Web panel, no game audience | No |
| Unified chat with replies | **Yes, inside OBS** | Separate web app | No |
| Unified events center | **Yes, inside OBS** | External web panel | No |
| Encrypted cloud backup | **Yes (zero-knowledge AES-256)** | No | No |
| Video signal privacy | **100% private, direct to platforms** | Relayed through their servers | 100% private |

## FAQ

<details>
<summary><b>Does multistreaming really use no extra GPU?</b></summary>

Yes. OBS encodes each frame once, and the plugin clones that compressed packet and sends it in parallel to the other platforms. Only your upload bandwidth is shared.
</details>

<details>
<summary><b>How much upload speed do I need?</b></summary>

Your total bitrate is the sum of all active destinations. A stable 50–100 Mbps upload connection is more than enough for most setups.
</details>

<details>
<summary><b>Does it open extra windows or run a separate app?</b></summary>

No. It is a native OBS plugin: everything runs as dockable panels inside OBS, with no Electron windows.
</details>

<details>
<summary><b>Can anyone read my stream keys in the cloud backup?</b></summary>

No. Data is encrypted locally with AES-256-GCM before it leaves your PC, using your Twitch identity and an optional PIN. Not even Steamify's servers can read your keys.
</details>

## About this repository

This repository only hosts the **official public releases and installers**. There is no source code here. Each release is built and published automatically by CI from the private source repository, with the installer's SHA256 checksum in the release notes.

## Support the project

Steamify Live is free and independently maintained by **Jefferson Oliveira ([@JeffNaPlay](https://livepix.gg/jeffnaplay))** for the creator community. Voluntary donations help keep the cloud infrastructure running and fund new updates.

[![LivePix](https://img.shields.io/badge/Donate-LivePix-ff6f00?style=for-the-badge&logo=ko-fi&logoColor=white)](https://livepix.gg/jeffnaplay)

## Links

- 🌐 Website: <https://live.steamify.com.br>
- 📦 Releases: <https://github.com/fjefferson/steamify-live-releases/releases>
- ✉️ Contact: oliveirjefferson@gmail.com
