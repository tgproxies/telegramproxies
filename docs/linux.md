<div align="center">

# 🐧 TgProxies — Linux Documentation

### Installation, Configuration & Troubleshooting

[![Bale](https://img.shields.io/badge/Bale-@tgproxies-26A5E4?style=for-the-badge)](https://web.bale.ai/@tgproxies)
![Platform](https://img.shields.io/badge/Platform-Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![Documentation](https://img.shields.io/badge/Documentation-Linux-blue?style=for-the-badge)

</div>

---

## 📖 Overview

This guide explains how to use **TgProxies** configurations on Linux devices.

TgProxies provides lists of proxy configurations for compatible client applications. The steps below cover choosing a client, installing it, importing a configuration, connecting, and troubleshooting common issues.

**Linux client downloads:** [`client/linux/README.md`](../client/linux/README.md)

---

## 📥 1. Choose a Linux Client

Different applications support different protocols and configuration formats.

| Client | Official download |
|---|---|
| v2rayA | [GitHub Releases](https://github.com/v2rayA/v2rayA/releases) |
| Hiddify | [GitHub Releases](https://github.com/hiddify/hiddify-app/releases) |
| Clash Verge Rev | [GitHub Releases](https://github.com/clash-verge-rev/clash-verge-rev/releases) |
| sing-box | [GitHub Releases](https://github.com/SagerNet/sing-box/releases) |
| mihomo | [GitHub Releases](https://github.com/MetaCubeX/mihomo/releases) |
| Shadowsocks-rust | [GitHub Releases](https://github.com/shadowsocks/shadowsocks-rust/releases) |

Always check the application's documentation and release notes to confirm protocol compatibility, Linux distribution requirements, and supported CPU architectures.

---

## 🔗 2. Find a Configuration

TgProxies stores configurations in the repository's `config/` directory.

| Protocol | Configuration file |
|---|---|
| VLESS | [`vless.txt`](../config/vless.txt) |
| VMess | [`vmess.txt`](../config/vmess.txt) |
| Shadowsocks | [`ss.txt`](../config/ss.txt) |
| Trojan | [`trojan.txt`](../config/trojan.txt) |
| All configurations | [`all.txt`](../config/all.txt) |

Select a protocol supported by your chosen client.

> **Important:** These files may contain individual configuration links rather than a subscription URL. Import methods depend on the format and the application.

---

## 📦 3. Install the Client

The installation method depends on the client and your Linux distribution.

1. Open the official download page for your chosen application.
2. Select a package compatible with your distribution and CPU architecture.
3. Download the appropriate package or archive.
4. Follow the installation instructions provided by the developer.
5. Install any required dependencies using your distribution's package manager.
6. Open the application.

Some clients provide AppImage, Flatpak, Debian packages, RPM packages, or standalone binaries. Availability varies by project.

> ⚠️ **Security warning:** Download applications from official project sources. Do not run unfamiliar installation scripts or binaries with administrator privileges.

---

## ⚙️ 4. Import a Configuration

The exact steps depend on your client and the configuration format.

### Method A — Import a share link

1. Open the relevant configuration file in TgProxies.
2. Copy a complete supported configuration link.
3. Open your proxy client.
4. Use its import-from-clipboard, add-server, or equivalent option.
5. Review the imported server details.
6. Save the configuration.

### Method B — Import a configuration file

If the client supports file import:

1. Download the configuration file.
2. Open the client.
3. Select its import-from-file option.
4. Choose the downloaded file.
5. Confirm the import.

If the client cannot import a text file containing multiple share links, try importing an individual configuration entry.

### Method C — Import a subscription

If a trusted provider supplies a subscription URL and your client supports subscriptions:

1. Open the subscription management section.
2. Add the subscription URL.
3. Update the subscription.
4. Select an available configuration.

**Do not treat a plain text list of individual proxy links as a subscription URL unless the client explicitly supports that format.**

---

## 🌐 5. Connect to a Server

1. Select an imported configuration.
2. Start the connection.
3. Configure the system proxy if you want compatible applications to use it.
4. If required, configure TUN mode or transparent proxy routing according to the client's documentation.
5. Grant administrator or network capabilities only when necessary and when you trust the software.
6. Test a website or application.

### 🖥️ System Proxy vs. TUN Mode

| Mode | Description |
|---|---|
| System Proxy | Routes traffic from applications that respect the desktop environment's proxy settings. |
| TUN Mode | Uses a virtual network interface to route traffic from more applications. |
| Transparent Proxy | Routes traffic through configured network rules; setup varies by client and distribution. |

Linux desktop environments and applications do not all use the same proxy settings. TUN mode and transparent proxy configurations may require additional permissions and networking components.

A successful connection does not guarantee that every website or application will work.

---

## 🧩 6. Protocol Overview

| Protocol | Description |
|---|---|
| VLESS | A proxy protocol commonly used with compatible Xray-based clients. |
| VMess | A proxy protocol supported by compatible V2Ray/Xray clients. |
| Shadowsocks | An encrypted proxy protocol with broad client support. |
| Trojan | A proxy protocol designed to carry traffic through TLS-based connections. |

Support varies by application and version. Always verify compatibility before importing a configuration.

---

## 🛠️ 7. Troubleshooting

<details>
<summary><strong>The configuration does not import</strong></summary>

- Confirm that the link or file is complete.
- Verify that the client supports the protocol.
- Use the correct import method for the format.
- Check whether the configuration contains unsupported options.
- Try importing one configuration entry instead of the entire file.
- Check the client's logs for parsing errors.

</details>

<details>
<summary><strong>The client cannot connect</strong></summary>

- Confirm that your computer has internet access without the proxy.
- Try a different configuration.
- Check whether the server details are still valid.
- Verify your system's date and time.
- Review the client's logs for connection errors.
- Check whether your firewall or network settings are blocking the connection.

</details>

<details>
<summary><strong>The client connects, but websites do not load</strong></summary>

- Check DNS and routing settings.
- Verify the desktop environment's system proxy settings.
- Check whether the application ignores system proxy settings.
- Review TUN mode or transparent proxy rules if you use them.
- Test more than one destination.
- Check whether another proxy application is interfering.

</details>

<details>
<summary><strong>The application requires root or administrator privileges</strong></summary>

- Check the official documentation to understand why.
- Network interfaces, routing rules, and transparent proxy features may require elevated permissions.
- Grant only the permissions required for the feature you intend to use.
- Avoid running the entire application as root unless its documentation specifically requires it.

</details>

<details>
<summary><strong>The application fails to start</strong></summary>

- Verify that the package matches your Linux distribution and architecture.
- Check whether required dependencies are installed.
- Review the application's logs or terminal output.
- Check executable permissions for standalone binaries.
- Consult the official installation instructions.

</details>

<details>
<summary><strong>The connection is slow or unstable</strong></summary>

- Try another configuration.
- Check your underlying internet connection.
- Test at different times.
- Review connection logs for timeouts or DNS failures.
- Check whether the selected protocol is supported by your client.
- Remember that server availability and performance can change.

</details>

---

## 🔐 8. Security & Privacy

- Download client applications from official sources.
- Do not publicly share private subscription URLs, credentials, or sensitive configuration data.
- A proxy does not guarantee anonymity or prevent all tracking.
- A proxy server operator may be able to observe some connection metadata or unencrypted traffic.
- Be cautious when granting root privileges or modifying firewall and routing rules.
- Keep your operating system and proxy client updated.
- Remove configurations you no longer trust or need.

Only connect to servers and use configurations that you are authorized to use.

---

## ❓ 9. Frequently Asked Questions

<details>
<summary><strong>Which Linux client should I use?</strong></summary>

Choose a client that supports your configuration's protocol and format. See the [Linux client list](../client/linux/README.md) for download links.

</details>

<details>
<summary><strong>Why does one configuration work while another does not?</strong></summary>

Servers can become unavailable, expire, or have different routing and protocol requirements. Try another configuration and check the client's error logs.

</details>

<details>
<summary><strong>Can I import every protocol into every client?</strong></summary>

No. Each client supports a specific set of protocols and formats. Consult the client's official documentation.

</details>

<details>
<summary><strong>Why does the proxy work in one application but not another?</strong></summary>

Some Linux applications ignore desktop system proxy settings. Check the application's proxy support or use a compatible routing mode supported by your client.

</details>

<details>
<summary><strong>Does TgProxies develop these applications?</strong></summary>

No. TgProxies links to third-party client projects and provides repository documentation and configuration lists.

</details>

<details>
<summary><strong>Are all listed configurations guaranteed to work?</strong></summary>

No. Availability, speed, compatibility, and reliability can change. A configuration should be tested before relying on it.

</details>

---

## 📚 10. Related Documentation

- [Linux Clients](../client/linux/README.md)
- [Android Clients](../client/apk/README.md)
- [Windows Clients](../client/windows/README.md)
- [iOS Clients](../client/ios/README.md)
- [All Configurations](../config/all.txt)
- [Repository Home](../README.md)

---

## 📢 Official Community

[![Join TgProxies on Bale](https://img.shields.io/badge/Join%20TgProxies-Bale%20Messenger-26A5E4?style=for-the-badge)](https://web.bale.ai/@tgproxies)

**TgProxies — Configurations, Clients, and Documentation.**
