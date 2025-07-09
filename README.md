# Pwnagotchi Packet Sniffer and Wireshark Analysis

A passive WPA handshaking sniffer and traffic analyzer built using a custom-configured **Pwnagotchi** running on a **Raspberry Pi Zero W** with a **Waveshare 2.13-inch e-Paper Display (Version 2)**. This project demonstrates automated packet capture, plugin extension, and offline analysis using Wireshark.

---

## 📦 Project Overview

This project configures a custom Pwnagotchi instance to:

- Autonomously sniff WPA handshakes using bettercap.
- Extend functionality using custom `.toml` configuration.
- Use additional plugins like `age` and `exp` to simulate AI-like growth.
- Collect and store `.pcap` files for offline inspection.
- Perform traffic feature analysis in **Wireshark** to examine EAPOL handshakes and other characteristics.

---

## 🛠️ Hardware Used

| Component                         | Description                                     |
|----------------------------------|-------------------------------------------------|
| Raspberry Pi Zero W              | Lightweight, low-power board for Pwnagotchi    |
| Waveshare 2.13" e-Paper Display  | Version 2, used to display Pwnagotchi face UI  |
| microSD Card                     | At least 8GB with flashed Pwnagotchi image     |
| Power Bank                       | Portable power supply for on-the-go operation  |

---

## 🧰 Software & Configuration

### 🔹 Pwnagotchi Version

- Based on [Pwnagotchi](https://pwnagotchi.ai/) image for Pi Zero W
- Custom `.toml` configuration located in `/etc/pwnagotchi/config.toml`

### 🔹 Key Config Changes

```toml
main.name = "IshaanBot"
main.lang = "en"
ui.display.enabled = true
ui.display.type = "waveshare_v2"
plugins.age.enabled = true
plugins.exp.enabled = true
