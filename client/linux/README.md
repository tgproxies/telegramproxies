<div align="center">

# 🐧 TgProxies — Linux Clients

### Proxy & VPN Applications for Linux

*Official downloads • Multiple protocols • Easy setup*

<a href="https://web.bale.ai/@tgproxies">
<img src="https://img.shields.io/badge/Bale-@tgproxies-26A5E4?style=for-the-badge" alt="Bale Channel">
</a>
<img src="https://img.shields.io/badge/Platform-Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black" alt="Linux">
<img src="https://img.shields.io/badge/Formats-DEB%20%7C%20RPM%20%7C%20AppImage-blue?style=for-the-badge" alt="Package formats">

</div>

---

## 📖 About

Welcome to the Linux client directory of **TgProxies**!

This page lists proxy and VPN client applications for Linux distributions. Use a compatible client to import configurations from the [`config/`](../../config/) directory.

> **Note:** TgProxies links to official project releases whenever possible. These applications are third-party projects and are not developed or endorsed by TgProxies.

---

## 📥 Available Clients

### 1. Hiddify

<a href="https://github.com/hiddify/hiddify-app/releases">
<img src="https://img.shields.io/badge/Download-Hiddify-3B82F6?style=for-the-badge&logo=linux&logoColor=white" alt="Download Hiddify">
</a>

A cross-platform client designed to simplify proxy configuration and connection management.

- **Platform:** Linux and other supported platforms
- **Download:** [GitHub Releases](https://github.com/hiddify/hiddify-app/releases)
- **Best for:** Users who prefer a graphical interface.

### 2. Clash Verge Rev

<a href="https://github.com/clash-verge-rev/clash-verge-rev/releases">
<img src="https://img.shields.io/badge/Download-Clash%20Verge%20Rev-FF9800?style=for-the-badge&logo=linux&logoColor=white" alt="Download Clash Verge Rev">
</a>

A desktop client for managing compatible Clash and Mihomo configurations.

- **Platform:** Linux and other supported platforms
- **Download:** [GitHub Releases](https://github.com/clash-verge-rev/clash-verge-rev/releases)
- **Best for:** Users with compatible Clash-format configuration files.

### 3. NekoRay

<a href="https://github.com/MatsuriDayo/nekoray/releases">
<img src="https://img.shields.io/badge/Download-NekoRay-673AB7?style=for-the-badge&logo=linux&logoColor=white" alt="Download NekoRay">
</a>

A desktop proxy client based on sing-box and related networking components.

- **Platform:** Linux; check the release page for available builds
- **Download:** [GitHub Releases](https://github.com/MatsuriDayo/nekoray/releases)
- **Note:** The project may not receive ongoing updates. Check compatibility before installing.

### 4. v2rayA

<a href="https://github.com/v2rayA/v2rayA/releases">
<img src="https://img.shields.io/badge/Download-v2rayA-0078D4?style=for-the-badge&logo=linux&logoColor=white" alt="Download v2rayA">
</a>

A Linux-oriented proxy management application with a web-based interface.

- **Platform:** Linux
- **Download:** [GitHub Releases](https://github.com/v2rayA/v2rayA/releases)
- **Best for:** Users who want to manage proxy connections through a browser.

### 5. sing-box

<a href="https://github.com/SagerNet/sing-box/releases">
<img src="https://img.shields.io/badge/Download-sing--box-607D8B?style=for-the-badge&logo=linux&logoColor=white" alt="Download sing-box">
</a>

A networking platform supporting multiple proxy protocols. It can run as a command-line application or as part of a compatible graphical client.

- **Platform:** Linux and other supported platforms
- **Download:** [GitHub Releases](https://github.com/SagerNet/sing-box/releases)
- **Best for:** Advanced users who prefer command-line configuration.

### 6. Shadowsocks-rust

<a href="https://github.com/shadowsocks/shadowsocks-rust/releases">
<img src="https://img.shields.io/badge/Download-Shadowsocks--rust-2196F3?style=for-the-badge&logo=linux&logoColor=white" alt="Download Shadowsocks-rust">
</a>

A Rust implementation of Shadowsocks with Linux-compatible releases.

- **Platform:** Linux and other supported platforms
- **Download:** [GitHub Releases](https://github.com/shadowsocks/shadowsocks-rust/releases)
- **Best for:** Users who need a Shadowsocks-compatible client or service.

---

## 📦 Installation Guide

Installation depends on the application and your Linux distribution.

### Debian / Ubuntu

For a project that provides a `.deb` package:

```bash
sudo apt install ./package-name.deb
```

Replace `package-name.deb` with the actual downloaded filename.

### Fedora / RHEL-based distributions

For a project that provides an `.rpm` package:

```bash
sudo dnf install ./package-name.rpm
```

Replace `package-name.rpm` with the actual downloaded filename.

### AppImage

If the project provides an AppImage:

```bash
chmod +x ./application.AppImage
./application.AppImage
```

Replace `application.AppImage` with the actual filename. Some distributions may require additional FUSE support.

### Portable archives

For a downloaded archive, extract it using your file manager or a suitable command-line tool. Follow the application's official installation instructions.

> **Important:** These are general examples, not universal installation commands. Always check the official documentation for package requirements and installation steps.

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

> **Compatibility:** Not every client supports every protocol or share-link format. Check the client's documentation before importing a configuration.

---

## 🛠️ Troubleshooting

<details>
<summary><strong>The application will not launch</strong></summary>

- Verify that you downloaded a build compatible with your CPU architecture and distribution.
- Check whether the application requires additional libraries or dependencies.
- If using an AppImage, confirm that it is executable.
- Download a fresh copy from the official release page if the file appears corrupted.

</details>

<details>
<summary><strong>Permission denied</strong></summary>

- Check the file permissions.
- For an AppImage, use `chmod +x` as shown above.
- Avoid running applications as root unless the official instructions specifically require it.

</details>

<details>
<summary><strong>The configuration cannot be imported</strong></summary>

- Verify that the client supports the protocol.
- Make sure the complete configuration was copied.
- Check whether the client expects a share link, subscription URL, or configuration file.

</details>

<details>
<summary><strong>The client connects but websites do not load</strong></summary>

- Try another configuration.
- Verify that the server is online and the configuration is still valid.
- Check the application's routing, DNS, and system proxy settings.
- Review firewall rules and conflicts with other VPN applications.

</details>

---

## 🔒 Security Notice

- Download software from official project sources.
- Avoid modified packages from unknown websites.
- Do not publish private keys, credentials, or personal subscription URLs.
- A proxy does not guarantee complete anonymity or prevent all tracking.
- Keep client software updated when maintained releases are available.

---

## 📢 Official Community

<div align="center">

<a href="https://web.bale.ai/@tgproxies">
<img src="https://img.shields.io/badge/Join%20TgProxies-Bale%20Messenger-26A5E4?style=for-the-badge" alt="Join TgProxies on Bale">
</a>

<br><br>

**TgProxies — Configurations, Clients, and Documentation.**

</div>
