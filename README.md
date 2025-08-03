# ESP32 Marauder Web Flasher

---

## 🇵🇱 ESP32 Marauder – Webowy Flasher

To narzędzie umożliwia łatwe flashowanie firmware'u **ESP32 Marauder** bez instalowania żadnego dodatkowego oprogramowania – wszystko odbywa się w przeglądarce.

> ⚠️ **To repozytorium zawiera jedynie flasher – nie jestem autorem firmware.**  
> Oryginalne oprogramowanie pochodzi z projektu:  
> 👉 https://github.com/justcallmekoko/ESP32Marauder

---

### 📦 Zawartość repozytorium

- `index.html` – interfejs użytkownika z przyciskiem „Install”
- `manifest.json` – konfiguracja flashowania (automatycznie aktualizowana)
- Pliki binarne (`.bin`) niezbędne do flashowania:
  - `boot_app0.bin`
  - `esp32_marauder.ino.bootloader.bin`
  - `esp32_marauder.ino.partitions.bin`
  - `esp32_marauder_<wersja>_2usb.bin`

---

### 🚀 Jak korzystać

1. Wejdź na stronę 
   https://marautech.github.io/ESP32-Cyd-Marauder-WebFlasher
2. Podłącz swoje ESP32 przez USB
3. Kliknij **Install**
4. Gotowe! Oprogramowanie zostanie wgrane automatycznie

---

### 🛠 Wymagania

- Przeglądarka z obsługą Web Serial (Chrome, Edge, Opera)
- ESP32 z USB

---
### 🙏 Credits

- [ESP32 Marauder](https://github.com/justcallmekoko/ESP32Marauder) – Autor Oprogramowania


## 🇬🇧 ESP32 Marauder – Web Flasher

This is a simple web tool for flashing **ESP32 Marauder firmware** directly from your browser – no drivers or software required.

> ⚠️ **This repository contains only the flasher – I am not the author of the firmware.**  
> The official firmware is available at:  
> 👉 https://github.com/justcallmekoko/ESP32Marauder

---

### 📦 Repository contents

- `index.html` – user interface with the install button
- `manifest.json` – firmware flashing config (auto-updated)
- Flashing files (`.bin`) included:
  - `boot_app0.bin`
  - `esp32_marauder.ino.bootloader.bin`
  - `esp32_marauder.ino.partitions.bin`
  - `esp32_marauder_<version>_2usb.bin`

---

### 🚀 How to use

1. Open the site
      https://marautech.github.io/ESP32-Cyd-Marauder-WebFlasher
2. Connect your ESP32 via USB
3. Click **Install**
4. The firmware will be flashed automatically

---

### 🛠 Requirements

- Browser with Web Serial API support (Chrome, Edge, Opera)
- USB-connected ESP32 board

---

### 🙏 Credits

- [ESP32 Marauder](https://github.com/justcallmekoko/ESP32Marauder) – firmware author
