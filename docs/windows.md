<div align="center">

# 💻 TgProxies — Windows Documentation

### Installation, Configuration & Troubleshooting

[![Bale](https://img.shields.io/badge/Bale-@tgproxies-26A5E4?style=for-the-badge)](https://web.bale.ai/@tgproxies)
![Platform](https://img.shields.io/badge/Platform-Windows-0078D4?style=for-the-badge&logo=windows&logoColor=white)
![Documentation](https://img.shields.io/badge/Documentation-Windows-blue?style=for-the-badge)

</div>

---

## 📖 Overview

This guide explains how to use **TgProxies** configurations on Windows devices.

TgProxies provides lists of proxy configurations for compatible client applications. The steps below cover choosing a client, downloading it, importing a configuration, connecting, and troubleshooting common issues.

**Windows client downloads:** [\`client/windows/README.md\`](../client/windows/README.md)

---

## 📥 1. Choose a Windows Client

Different applications support different protocols and configuration formats.

| Client | Official download |
|---|---|
| v2rayN | [GitHub Releases](https://github.com/2dust/v2rayN/releases) |
| Hiddify | [GitHub Releases](https://github.com/hiddify/hiddify-app/releases) |
| Clash Verge Rev | [GitHub Releases](https://github.com/clash-verge-rev/clash-verge-rev/releases) |
| NekoRay | [GitHub Releases](https://github.com/MatsuriDayo/nekoray/releases) |
| sing-box | [GitHub Releases](https://github.com/SagerNet/sing-box/releases) |
| Shadowsocks-Windows | [GitHub Releases](https://github.com/shadowsocks/shadowsocks-windows/releases) |

Always check the application's documentation and release notes to confirm protocol compatibility and Windows requirements.

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

## 📥 3. Install the Client

1. Open the official download page for your chosen application.
2. Download a release compatible with your Windows version and system architecture.
3. If the download is an installer, open it and follow the installation instructions.
4. If the download is a portable archive, extract it and follow the developer's instructions.
5. Complete any required setup.
6. Open the application.

For security, download applications only from official project sources that you trust. Avoid running unknown executables or granting unnecessary administrator permissions.

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
3. Enable the system proxy option if you want compatible Windows applications to use it.
4. If needed, enable TUN mode according to the client's documentation.
5. Wait for the client to report a successful connection.
6. Test a website or application.

System proxy settings may not affect every application. TUN mode can route traffic from more applications, but may require additional permissions and configuration.

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
- Try another compatible client if necessary.

</details>

<details>
<summary><strong>The client cannot connect</strong></summary>

- Confirm that your computer has internet access without the proxy.
- Try a different configuration.
- Check whether the server details are still valid.
- Verify that your computer's date and time are correct.
- Check the client's connection logs for useful error messages.
- Check whether your firewall or network is blocking the connection.

</details>

<details>
<summary><strong>The client connects, but websites do not load</strong></summary>

- Check DNS and routing settings.
- Verify that the application is configured to route traffic as intended.
- Check whether the Windows system proxy is enabled when required.
- Review TUN mode settings if you use them.
- Disconnect other proxy applications that might conflict.
- Test more than one destination to determine whether the problem affects all traffic.

</details>

<details>
<summary><strong>Only some applications use the proxy</strong></summary>

- Check whether those applications respect Windows system proxy settings.
- Review the client's routing rules.
- Consider TUN mode if the client supports it and you need broader traffic routing.
- Check whether another application is overriding the proxy settings.

</details>

<details>
<summary><strong>The connection is slow or unstable</strong></summary>

- Try another configuration.
- Check the stability of your underlying internet connection.
- Test at different times.
- Check the client logs for timeouts or connection errors.
- Remember that server availability and performance can change.

</details>

<details>
<summary><strong>The application requires administrator permissions</strong></summary>

- Check the application's official documentation to understand why.
- TUN mode and virtual network adapters may require elevated permissions.
- Run the application as administrator only when necessary and when you trust its source.
- Do not disable Windows security protections indiscriminately.

</details>

---

## 🔐 8. Security & Privacy

- Download client applications from official sources.
- Do not publicly share private subscription URLs, credentials, or sensitive configuration data.
- A proxy does not guarantee anonymity or prevent all tracking.
- A proxy server operator may be able to observe some connection metadata or unencrypted traffic.
- Be cautious when granting administrator permissions or installing network drivers.
- Keep your client software updated.
- Remove configurations you no longer trust or need.

Only connect to servers and use configurations that you are authorized to use.

---

## ❓ 9. Frequently Asked Questions

<details>
<summary><strong>Which Windows client should I use?</strong></summary>

Choose a client that supports your configuration's protocol and format. See the [Windows client list](../client/windows/README.md) for download links.

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
<summary><strong>What is the difference between system proxy and TUN mode?</strong></summary>

System proxy settings affect applications that respect Windows proxy configuration. TUN mode can route traffic from more applications through a virtual network interface, but may require extra permissions.

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

- [Windows Clients](../client/windows/README.md)
- [Android Clients](../client/apk/README.md)
- [Linux Clients](../client/linux/README.md)
- [iOS Clients](../client/ios/README.md)
- [All Configurations](../config/all.txt)
- [Repository Home](../README.md)

---

## 📢 Official Community

[![Join TgProxies on Bale](https://img.shields.io/badge/Join%20TgProxies-Bale%20Messenger-26A5E4?style=for-the-badge)](https://web.bale.ai/@tgproxies)

**TgProxies — Configurations, Clients, and Documentation.**
