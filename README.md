# Pwnagotchi Packet Sniffer and Wireshark Analysis

A passive WPA handshaking sniffer and traffic analyzer built using a custom-configured **Pwnagotchi** running on a **Raspberry Pi Zero W** with a **Waveshare 2.13-inch e-Paper Display (Version 2)**. This project demonstrates automated packet capture, plugin extension, and offline analysis using Wireshark.

---

## Project Overview

This project configures a custom Pwnagotchi instance to:

- Autonomously sniff WPA handshakes using bettercap.
- Extend functionality using custom `.toml` configuration.
- Use additional plugins like `age` and `exp` to simulate AI-like growth.
- Collect and store `.pcap` files for offline inspection.
- Perform traffic feature analysis in **Wireshark** to examine EAPOL handshakes and other characteristics.

---

## Hardware Used

|           Component              |                   Description                   |
|----------------------------------|-------------------------------------------------|
| Raspberry Pi Zero W              |  Lightweight, low-power board for Pwnagotchi    |
| Waveshare 2.13" e-Paper Display  |  Version 2, used to display Pwnagotchi face UI  |
| microSD Card                     |  64GB with flashed Pwnagotchi image             |
| Power                            | Via a 5V 3A power Adaptor and a micro USB Cable |

---

## Software & Configuration

### Pwnagotchi Version 2.6.4

- Based on [Pwnagotchi](https://pwnagotchi.ai/) image for Pi Zero W
- Custom `.toml` configuration located in `nano /etc/pwnagotchi/config.toml`


### Steps followed:

The steps to do this project are as follows
(the work is a little derivative and can be found on any youtube tutorial):

1. Get the latest Pwnagotchi image(currently 2.9.5.3)by Jayfelony and 
download it on your local machine.

2. Flash the image file on a microSD card by using either of the two,
Rpi imager or balena Etcher

3. Insert the SD card into the Pwnagotchi with the 2.13 inch waveshare v4 plugged 
onto the Rpi

4. Let the Rpi boot for a while, for the first run, i would suggest to boot 
using your laptops power USB port and the Rpi's Data port to SSH into the Rpi

5. The default ip assigned to the Pwnagotchi is 10.0.0.2

6. To SSH into the Pwnagotchi, you will no to change the IP Address and obviously
the subnet of your Laptop/device.

7. After SSHing into the Rpi, we would want to configure the Toml file using
sudo nano /etc/pwnagotchi/config.toml
(not the Defaults.toml as it will be always auto-generated on bootup).

8. The next steps include giving the Pi a Wi-fi connection and Bluetooth 
