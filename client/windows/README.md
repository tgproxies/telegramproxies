<div align="center">

# 🖥️ TgProxies — Windows Clients

### Proxy & VPN Applications for Windows

*Official downloads • Multiple protocols • Easy configuration*

<a href="https://web.bale.ai/@tgproxies">
<img src="https://img.shields.io/badge/Bale-@tgproxies-26A5E4?style=for-the-badge" alt="Bale Channel">
</a>
<img src="https://img.shields.io/badge/Platform-Windows-0078D4?style=for-the-badge&logo=windows&logoColor=white" alt="Windows">
<img src="https://img.shields.io/badge/Architecture-x64%20%7C%20ARM64-blue?style=for-the-badge" alt="Architecture">

</div>

---

## 📖 About

Welcome to the Windows client directory of **TgProxies**!

This page lists proxy and VPN client applications for Windows. Use a compatible client to import configurations from the [`config/`](../../config/) directory.

> **Note:** TgProxies links to official project releases whenever possible. These applications are third-party projects and are not developed or endorsed by TgProxies.

---

## 📥 Available Clients

### 1. v2rayN

<a href="https://github.com/2dust/v2rayN/releases">
<img src="https://img.shields.io/badge/Download-v2rayN-0078D4?style=for-the-badge&logo=windows&logoColor=white" alt="Download v2rayN">
</a>

A Windows proxy client with support for multiple proxy protocols through compatible cores.

- **Platform:** Windows
- **Download:** [GitHub Releases](https://github.com/2dust/v2rayN/releases)
- **Best for:** Managing and importing compatible proxy configurations.

### 2. Hiddify

<a href="https://github.com/hiddify/hiddify-app/releases">
<img src="https://img.shields.io/badge/Download-Hiddify-3B82F6?style=for-the-badge&logo=windows&logoColor=white" alt="Download Hiddify">
</a>

A cross-platform client designed to simplify proxy configuration and connection management.

- **Platform:** Windows and other supported platforms
- **Download:** [GitHub Releases](https://github.com/hiddify/hiddify-app/releases)
- **Best for:** Users who prefer a straightforward interface.

### 3. NekoRay

<a href="https://github.com/MatsuriDayo/nekoray/releases">
<img src="https://img.shields.io/badge/Download-NekoRay-673AB7?style=for-the-badge&logo=windows&logoColor=white" alt="Download NekoRay">
</a>

A desktop proxy client based on sing-box and related networking components.

- **Platform:** Windows and Linux releases may be available
- **Download:** [GitHub Releases](https://github.com/MatsuriDayo/nekoray/releases)
- **Note:** Check the release page for availability and compatibility. The project may not receive ongoing updates.

### 4. Clash Verge Rev

<a href="https://github.com/clash-verge-rev/clash-verge-rev/releases">
<img src="https://img.shields.io/badge/Download-Clash%20Verge%20Rev-FF9800?style=for-the-badge&logo=windows&logoColor=white" alt="Download Clash Verge Rev">
</a>

A desktop client for managing compatible Clash and Mihomo configurations.

- **Platform:** Windows and other supported platforms
- **Download:** [GitHub Releases](https://github.com/clash-verge-rev/clash-verge-rev/releases)
- **Best for:** Users with compatible Clash-format configuration files.

### 5. sing-box

<a href="https://github.com/SagerNet/sing-box/releases">
<img src="https://img.shields.io/badge/Download-sing--box-607D8B?style=for-the-badge&logo=windows&logoColor=white" alt="Download sing-box">
</a>

A networking platform that supports multiple proxy protocols. It can be used directly through its command-line interface or with a compatible graphical client.

- **Platform:** Windows and other supported platforms
- **Download:** [GitHub Releases](https://github.com/SagerNet/sing-box/releases)
- **Best for:** Advanced users who want to manage configurations directly.

### 6. Shadowsocks-Windows

<a href="https://github.com/shadowsocks/shadowsocks-windows/releases">
<img src="https://img.shields.io/badge/Download-Shadowsocks--Windows-2196F3?style=for-the-badge&logo=windows&logoColor=white" alt="Download Shadowsocks-Windows">
</a>

A Windows client specifically for compatible Shadowsocks configurations.

- **Platform:** Windows
- **Download:** [GitHub Releases](https://github.com/shadowsocks/shadowsocks-windows/releases)
- **Best for:** Users who only need Shadowsocks support.

---

## 📲 Installation Guide

1. Open the official release page for your chosen application.
2. Download the Windows version compatible with your system.
3. Extract the archive if the download is a ZIP file.
4. Run the application or installer as instructed by the project.
5. If Windows Defender or SmartScreen displays a warning, verify the publisher and downloaded file before deciding whether to continue.
6. Import a compatible proxy configuration.
7. Connect and test your internet connection.

**Tip:** Avoid running unknown executables as administrator. Only grant elevated permissions when they are necessary and you trust the application.

---

## 🔗 TgProxies Configuration Lists

Browse the configuration files in this repository:

| Protocol | Configuration list |
|---|---|
| VLESS | [`vless.txt`](../../config/vless.txt) |
| VMess | [`vmess.txt`](../../config/vmess.txt) |
| Shadowsocks | [`ss.txt`](../../config/ss.txt) |
| Trojan | [`trojan.txt`](../../config/trojan.txt) |
| All configurations | [`all.txt`](../../config/all.txt) |

> **Compatibility:** Each client supports a different set of protocols and configuration formats. Check the application's documentation before importing a configuration.

---

## 🛠️ Troubleshooting

<details>
<summary><strong>The application will not start</strong></summary>

- Check that the download matches your Windows architecture.
- Extract the complete archive before running a portable application.
- Check the project's documentation for required runtimes or dependencies.
- Download a fresh copy from the official release page if the file appears corrupted.

</details>

<details>
<summary><strong>Windows blocks the application</strong></summary>

- Verify that the file came from the official project.
- Check the publisher, digital signature, and release information when available.
- Do not disable antivirus protection simply to run an unfamiliar program.

</details>

<details>
<summary><strong>The configuration cannot be imported</strong></summary>

- Verify that the client supports the configuration's protocol.
- Make sure the complete configuration was copied.
- Check whether the application expects a URL, a share link, or a configuration file.

</details>

<details>
<summary><strong>The client connects but websites do not load</strong></summary>

- Try another configuration.
- Check whether the server is online and the configuration is still valid.
- Review the application's system proxy, TUN, or routing settings.
- Check for conflicts with other VPN clients or firewall rules.

</details>

---

## 🔒 Security Notice

- Download software from official project sources.
- Avoid repackaged or modified executables from unknown websites.
- Never publish private keys, credentials, or personal subscription URLs.
- A proxy does not guarantee complete anonymity or protection against tracking.
- Keep your client software updated when supported releases are available.

---

## 📢 Official Community

<div align="center">

<a href="https://web.bale.ai/@tgproxies">
<img src="https://img.shields.io/badge/Join%20TgProxies-Bale%20Messenger-26A5E4?style=for-the-badge" alt="Join TgProxies on Bale">
</a>

<br><br>

**TgProxies — Configurations, Clients, and Documentation.**

</div>
