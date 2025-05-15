# Disable M1–M6 Macro Keys on Razer BlackWidow V4 X in Linux (Python USB Script)

This project provides a simple Python script to **disable the M1–M6 macro keys** on the **Razer BlackWidow V4 X** keyboard (or similar models like the Ultimate Elite) when used on **Linux**, specifically tested on **Linux Mint**.

It communicates directly with the device over USB and sends a control transfer to turn off macro key functionality and their backlight.

---

## 🔧 Features

- Disables M1–M6 macro keys via USB command.
- Turns off the macro key backlight as a visual confirmation.
- Uses `pyusb` to send control messages to the keyboard.
- Safe to use: does not flash or alter firmware.
- Works on Linux Mint and similar distributions.

---

## ⚠️ Limitations

- **Takes a few seconds to activate after boot.**
- **Does not persist automatically across reboots** unless added to startup manually.
- Requires **root access** to communicate with USB devices.
- Only tested with **Razer BlackWidow V4 X** (USB ID: `1532:0293`).

---

## 🖥 Requirements

- Linux (tested on Linux Mint)
- Python 3
- `pyusb` library

---

## 📦 Installation

### 1. Install Dependencies

```bash
sudo apt update
sudo apt install python3 python3-pip
pip3 install pyusb
