<div align="center">

# 🍎 TgProxies — iOS Documentation

### Installation, Configuration & Troubleshooting

[![Bale](https://img.shields.io/badge/Bale-@tgproxies-26A5E4?style=for-the-badge)](https://web.bale.ai/@tgproxies)
![Platform](https://img.shields.io/badge/Platform-iOS-000000?style=for-the-badge&logo=apple&logoColor=white)
![Documentation](https://img.shields.io/badge/Documentation-iOS-blue?style=for-the-badge)

</div>

---

## 📖 Overview

This guide explains how to use **TgProxies** configurations on iPhone and iPad.

TgProxies provides lists of proxy configurations for compatible client applications. The steps below cover choosing a client, installing it, importing a configuration, connecting, and troubleshooting common issues.

**iOS client downloads:** [`client/ios/README.md`](../client/ios/README.md)

---

## 📥 1. Choose an iOS Client

Different applications support different protocols and configuration formats.

| Client | Official download |
|---|---|
| Shadowrocket | [Official Website](https://apps.apple.com/) |
| Streisand | [App Store](https://apps.apple.com/) |
| Hiddify | [Official Website](https://hiddify.com/) |
| sing-box | [GitHub Releases](https://github.com/SagerNet/sing-box/releases) |
| FoXray | [App Store](https://apps.apple.com/) |

App availability, pricing, regional restrictions, and supported protocols may vary. Search for the exact application in the App Store and verify the developer before installing it.

Always check the application's documentation and release notes to confirm protocol compatibility and iOS requirements.

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

## 📲 3. Install the Client

1. Open the App Store or the official project page for your chosen application.
2. Verify the application's name and developer.
3. Download and install the application.
4. Open it and complete any initial setup.
5. Review the permissions requested by the application.

Some clients are paid or available only in certain regions. Availability also depends on the application's current distribution method.

For security, prefer the App Store or official developer sources. Avoid installing configuration profiles or certificates from unknown sources.

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

1. Download the configuration file to your device.
2. Open the Files app.
3. Locate the downloaded file.
4. Use the Share menu or the application's import option.
5. Select your proxy client if it supports receiving the file.
6. Confirm the import.

Not every client can import a plain text file containing multiple share links. If the import fails, try importing an individual supported configuration entry.

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
3. Approve the iOS VPN configuration prompt if you trust the application.
4. Authenticate with your device if requested.
5. Wait for the client to report a successful connection.
6. Test a website or application.

iOS generally allows only one active system VPN connection at a time. Another VPN application or configuration may need to be disconnected first.

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

- Confirm that your device has internet access without the proxy.
- Try a different configuration.
- Check whether the server details are still valid.
- Verify that your device's date and time are correct.
- Check the client's connection logs for useful error messages.
- Disconnect other active VPN connections.

</details>

<details>
<summary><strong>The client connects, but websites do not load</strong></summary>

- Check the client's DNS and routing settings.
- Verify that the application is configured to route traffic as intended.
- Test more than one destination.
- Check whether the server is reachable and functioning.
- Review the client's logs for connection errors.

</details>

<details>
<summary><strong>The VPN disconnects unexpectedly</strong></summary>

- Check the client's connection settings.
- Keep the application updated.
- Review any on-demand VPN settings.
- Check whether another VPN application is attempting to connect.
- Restart the client and test another configuration.

</details>

<details>
<summary><strong>The application is unavailable in the App Store</strong></summary>

- Search for the exact application name.
- Check the developer's official website for current distribution information.
- Verify regional availability and device compatibility.
- Avoid downloading modified applications from untrusted websites.

</details>

<details>
<summary><strong>The VPN permission prompt does not appear</strong></summary>

- Open the client and try connecting again.
- Check the VPN section in iOS Settings.
- Review any existing VPN configurations.
- Follow the application's official troubleshooting instructions.

</details>

---

## 🔐 8. Security & Privacy

- Download client applications from official sources.
- Do not publicly share private subscription URLs, credentials, or sensitive configuration data.
- A proxy does not guarantee anonymity or prevent all tracking.
- A proxy server operator may be able to observe some connection metadata or unencrypted traffic.
- Be cautious when installing configuration profiles or certificates.
- Review VPN permissions and remove configurations you no longer trust or need.
- Keep iOS and your proxy client updated.

Only connect to servers and use configurations that you are authorized to use.

---

## ❓ 9. Frequently Asked Questions

<details>
<summary><strong>Which iOS client should I use?</strong></summary>

Choose a client that supports your configuration's protocol and format. See the [iOS client list](../client/ios/README.md) for download links.

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
<summary><strong>Why does iOS ask to add a VPN configuration?</strong></summary>

iOS requires user approval before an application can add or use many system VPN configurations. Approve the request only if you trust the application.

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

- [iOS Clients](../client/ios/README.md)
- [Android Clients](../client/apk/README.md)
- [Windows Clients](../client/windows/README.md)
- [Linux Clients](../client/linux/README.md)
- [All Configurations](../config/all.txt)
- [Repository Home](../README.md)

---

## 📢 Official Community

[![Join TgProxies on Bale](https://img.shields.io/badge/Join%20TgProxies-Bale%20Messenger-26A5E4?style=for-the-badge)](https://web.bale.ai/@tgproxies)

**TgProxies — Configurations, Clients, and Documentation.**
