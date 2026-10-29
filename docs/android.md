<div align="center">

# 📱 TgProxies — Android Documentation

### Installation, Configuration & Troubleshooting

[![Bale](https://img.shields.io/badge/Bale-@tgproxies-26A5E4?style=for-the-badge)](https://web.bale.ai/@tgproxies)
![Platform](https://img.shields.io/badge/Platform-Android-3DDC84?style=for-the-badge&logo=android&logoColor=white)
![Documentation](https://img.shields.io/badge/Documentation-Android-blue?style=for-the-badge)

</div>

---

## 📖 Overview

This guide explains how to use **TgProxies** configurations on Android devices.

TgProxies provides lists of proxy configurations for compatible client applications. The steps below cover choosing a client, downloading it, importing a configuration, connecting, and troubleshooting common issues.

**Android client downloads:** [`client/apk/README.md`](../client/apk/README.md)

---

## 📥 1. Choose an Android Client

Different applications support different protocols and configuration formats.

| Client | Official download |
|---|---|
| MahsaNG | [GitHub Releases](https://github.com/GFW-knocker/MahsaNG/releases) |
| v2rayNG | [GitHub Releases](https://github.com/2dust/v2rayNG/releases) |
| NekoBox for Android | [GitHub Releases](https://github.com/MatsuriDayo/NekoBoxForAndroid/releases) |
| Hiddify | [GitHub Releases](https://github.com/hiddify/hiddify-app/releases) |
| Clash Meta for Android | [GitHub Releases](https://github.com/MetaCubeX/ClashMetaForAndroid/releases) |

Always check the application's documentation and release notes to confirm protocol compatibility and Android requirements.

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

1. Open the official download page for your chosen application.
2. Download a release compatible with your device.
3. Open the downloaded APK.
4. If Android asks for permission to install unknown apps, verify the source before allowing installation.
5. Complete the installation.
6. Open the application.

For security, only install APKs from official project sources that you trust. Disable the installation permission afterward if you no longer need it.

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
3. Approve Android's VPN connection prompt if you trust the application.
4. Wait for the client to report a successful connection.
5. Test a website or application.

Android normally allows one active VPN service at a time. Another VPN application may need to be disconnected first.

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
- Try another compatible client if necessary.

</details>

<details>
<summary><strong>The client cannot connect</strong></summary>

- Confirm that your device has internet access without the proxy.
- Try a different configuration.
- Check whether the server details are still valid.
- Verify the device's date and time.
- Check the client's connection logs for useful error messages.

</details>

<details>
<summary><strong>The client connects, but websites do not load</strong></summary>

- Check DNS and routing settings.
- Verify that the application is configured to route traffic as intended.
- Check whether Android's battery restrictions are stopping the client.
- Disconnect other VPN applications.
- Test more than one destination to determine whether the problem affects all traffic.

</details>

<details>
<summary><strong>The VPN disconnects in the background</strong></summary>

- Review Android's battery optimization settings for the client.
- Check whether your device manufacturer applies additional background restrictions.
- Keep the application updated.
- Use only the background and always-on VPN options you actually need.

</details>

<details>
<summary><strong>APK installation is blocked</strong></summary>

- Confirm that the APK came from the official project release page.
- Verify that the APK supports your Android version and device architecture.
- Check available storage space.
- Avoid disabling device security protections to install an untrusted file.

</details>

---

## 🔐 8. Security & Privacy

- Download client applications from official sources.
- Do not publicly share private subscription URLs, credentials, or sensitive configuration data.
- A proxy does not guarantee anonymity or prevent all tracking.
- A proxy server operator may be able to observe some connection metadata or unencrypted traffic.
- Be cautious when granting VPN, accessibility, certificate, or other elevated permissions.
- Remove configurations you no longer trust or need.

Only connect to servers and use configurations that you are authorized to use.

---

## ❓ 9. Frequently Asked Questions

<details>
<summary><strong>Which Android client should I use?</strong></summary>

Choose a client that supports your configuration's protocol and format. See the [Android client list](../client/apk/README.md) for download links.

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
<summary><strong>Does TgProxies develop these applications?</strong></summary>

No. TgProxies links to third-party client projects and provides repository documentation and configuration lists.

</details>

<details>
<summary><strong>Are all listed configurations guaranteed to work?</strong></summary>

No. Availability, speed, compatibility, and reliability can change. A configuration should be tested before relying on it.

</details>

---

## 📚 Related Documentation

- [Android Clients](../client/apk/README.md)
- [Windows Clients](../client/windows/README.md)
- [Linux Clients](../client/linux/README.md)
- [iOS Clients](../client/ios/README.md)
- [All Configurations](../config/all.txt)
- [Repository Home](../README.md)

---

## 📢 Official Community

[![Join TgProxies on Bale](https://img.shields.io/badge/Join%20TgProxies-Bale%20Messenger-26A5E4?style=for-the-badge)](https://web.bale.ai/@tgproxies)

**TgProxies — Configurations, Clients, and Documentation.**
