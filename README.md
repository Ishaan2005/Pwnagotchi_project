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

|           Component              |                   Description                   |
|----------------------------------|-------------------------------------------------|
| Raspberry Pi Zero W              |  Lightweight, low-power board for Pwnagotchi    |
| Waveshare 2.13" e-Paper Display  |  Version 2, used to display Pwnagotchi face UI  |
| microSD Card                     |  64GB with flashed Pwnagotchi image             |
| Power                            | Via a 5V 3A power Adaptor and a micro USB Cable |

---

## 🧰 Software & Configuration

### 🔹 Pwnagotchi Version 2.6.4

- Based on [Pwnagotchi](https://pwnagotchi.ai/) image for Pi Zero W
- Custom `.toml` configuration located in `nano /etc/pwnagotchi/config.toml`


