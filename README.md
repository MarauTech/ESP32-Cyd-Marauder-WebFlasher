<div align="center">

# ESP32 Marauder Web Flasher

**Browser-based firmware installer for ESP32 and CYD (Cheap Yellow Display) boards.**

[![Launch Web Flasher](https://img.shields.io/badge/Launch-Web%20Flasher-2ea44f?style=for-the-badge&logo=google-chrome&logoColor=white)](https://marautech.github.io/ESP32-Cyd-Marauder-WebFlasher)

<br/>

[![GitHub Pages](https://img.shields.io/badge/Deployment-GitHub%20Pages-181717?style=flat-square&logo=github)](https://marautech.github.io/ESP32-Cyd-Marauder-WebFlasher)
[![Web Serial API](https://img.shields.io/badge/Protocol-Web%20Serial%20API-4285F4?style=flat-square&logo=googlechrome&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/API/Web_Serial_API)
[![Hardware](https://img.shields.io/badge/Target-ESP32%20CYD%20(2USB)-E7352C?style=flat-square&logo=espressif&logoColor=white)](https://github.com/justcallmekoko/ESP32Marauder)

<br/>

[English](#english) | [Polski](#polski)

</div>

---

## English

### <img src="https://api.iconify.design/octicon:info-16.svg" width="16" height="16" /> Overview

This project provides a browser-based firmware installer for **ESP32 Marauder** (configured for CYD / ESP32 dual USB boards). Utilizing the **Web Serial API**, you can flash your device directly from the browser without installing Arduino IDE, Python, or external drivers.

> [!WARNING]
> **Disclaimer:** This repository contains only the web flasher interface and pre-compiled binaries. I am not the author of the ESP32 Marauder firmware.  
> Official source code and documentation: [justcallmekoko/ESP32Marauder](https://github.com/justcallmekoko/ESP32Marauder)

### <img src="https://api.iconify.design/octicon:rocket-16.svg" width="16" height="16" /> Quick Start

1. Open the web tool: [ESP32 Marauder Web Flasher](https://marautech.github.io/ESP32-Cyd-Marauder-WebFlasher).
2. Connect your ESP32 board to your computer with a USB data cable.
3. Click **Install**.
4. Select the corresponding serial port in the browser prompt (such as `COM3` on Windows or `/dev/ttyUSB0` on Linux).
5. Wait for the flashing procedure to finish.

### <img src="https://api.iconify.design/octicon:file-directory-16.svg" width="16" height="16" /> Repository Contents

| File | Description |
| :--- | :--- |
| `index.html` | Web interface running the Web Serial flashing script |
| `boot_app0.bin` | ESP32 boot app partition binary |
| `esp32_marauder.ino.bootloader.bin` | Bootloader binary |
| `esp32_marauder.ino.partitions.bin` | Partition table definition |
| `esp32_marauder_<version>_2usb.bin` | Compiled Marauder firmware application binary |

### <img src="https://api.iconify.design/octicon:cpu-16.svg" width="16" height="16" /> Requirements

* **Browser:** Chromium-based browser supporting Web Serial API (Google Chrome, Microsoft Edge, Opera, Brave).
* **Hardware:** ESP32 board (specifically CYD / ESP32-2432S028R dual USB variant).
* **Connection:** USB cable with data lines (charging-only cables will not be detected).

### <img src="https://api.iconify.design/octicon:question-16.svg" width="16" height="16" /> Troubleshooting

<details>
<summary><b>Device not detected by the browser</b></summary>

1. Confirm that your USB cable supports data transfer, not only charging.
2. Install the appropriate USB-to-UART driver for your board:
   * [CH340 / CH341 Driver](https://learn.sparkfun.com/tutorials/how-to-install-ch340-drivers/all)
   * [CP210x Driver](https://www.silabs.com/developers/usb-to-uart-bridge-vcp-drivers)
</details>

<details>
<summary><b>Connection error during flashing</b></summary>

* Hold down the **BOOT** button on your ESP32 while clicking Install, then release it once the writing process begins.
* Close any software that may lock the COM port (such as Arduino Serial Monitor, Cura, PuTTY).
</details>

### <img src="https://api.iconify.design/octicon:heart-16.svg" width="16" height="16" /> Credits

* [justcallmekoko](https://github.com/justcallmekoko): Author of the official [ESP32 Marauder](https://github.com/justcallmekoko/ESP32Marauder) project.

---

## Polski

### <img src="https://api.iconify.design/octicon:info-16.svg" width="16" height="16" /> Opis projektu

Narzędzie umożliwia instalację oprogramowania **ESP32 Marauder** (wersja dla płytek CYD / ESP32 z podwójnym portem USB) bezpośrednio z poziomu przeglądarki. Dzięki technologii **Web Serial API** cały proces odbywa się bez potrzeby instalacji Arduino IDE, środowiska Python czy zewnętrznych programów.

> [!WARNING]
> **Zastrzeżenie prawne:** To repozytorium zawiera wyłącznie webowy interfejs instalatora oraz skompilowane pliki binarne. Nie jestem autorem oprogramowania ESP32 Marauder.  
> Oficjalny kod źródłowy oraz dokumentacja: [justcallmekoko/ESP32Marauder](https://github.com/justcallmekoko/ESP32Marauder)

### <img src="https://api.iconify.design/octicon:rocket-16.svg" width="16" height="16" /> Instrukcja instalacji

1. Otwórz instalator: [ESP32 Marauder Web Flasher](https://marautech.github.io/ESP32-Cyd-Marauder-WebFlasher).
2. Podłącz płytkę ESP32 do komputera kablem USB obsługującym przesył danych.
3. Kliknij przycisk **Install**.
4. Wybierz odpowiedni port szeregowy w oknie przeglądarki (np. `COM3` w systemie Windows lub `/dev/ttyUSB0` w systemie Linux).
5. Poczekaj na ukończenie procesu wgrywania oprogramowania.

### <img src="https://api.iconify.design/octicon:file-directory-16.svg" width="16" height="16" /> Zawartość repozytorium

| Plik | Opis |
| :--- | :--- |
| `index.html` | Interfejs webowy wykorzystujący protokół Web Serial |
| `boot_app0.bin` | Plik rozruchowy partycji aplikacji ESP32 |
| `esp32_marauder.ino.bootloader.bin` | Plik binarny bootloadera |
| `esp32_marauder.ino.partitions.bin` | Tabela podziału pamięci flash (partycje) |
| `esp32_marauder_<wersja>_2usb.bin` | Skompilowany plik binarny oprogramowania Marauder |

### <img src="https://api.iconify.design/octicon:cpu-16.svg" width="16" height="16" /> Wymagania

* **Przeglądarka:** Google Chrome, Microsoft Edge, Opera lub Brave (dowolna przeglądarka na silniku Chromium z obsługą Web Serial API).
* **Sprzęt:** Płytka ESP32 (wariant CYD / ESP32-2432S028R z 2x USB).
* **Kabel:** Przewód USB z liniami danych (kable służące wyłącznie do ładowania uniemożliwią wykrycie urządzenia).

### <img src="https://api.iconify.design/octicon:question-16.svg" width="16" height="16" /> Rozwiązywanie problemów

<details>
<summary><b>Przeglądarka nie wykrywa podłączonego urządzenia</b></summary>

1. Upewnij się, że kabel USB obsługuje transmisję danych, a nie tylko zasilanie.
2. Zainstaluj właściwe sterowniki konwertera USB-UART dla swojego systemu:
   * [Sterowniki CH340 / CH341](https://learn.sparkfun.com/tutorials/how-to-install-ch340-drivers/all)
   * [Sterowniki CP210x](https://www.silabs.com/developers/usb-to-uart-bridge-vcp-drivers)
</details>

<details>
<summary><b>Błąd połączenia podczas wgrywania</b></summary>

* Przytrzymaj przycisk **BOOT** na płytce ESP32 w momencie klikania przycisku Install, a po rozpoczęciu zapisu zwolnij go.
* Zamknij programy mogące blokować port szeregowy (np. monitor portu w Arduino IDE, Cura, PuTTY).
</details>

### <img src="https://api.iconify.design/octicon:heart-16.svg" width="16" height="16" /> Podziękowania

* [justcallmekoko](https://github.com/justcallmekoko): Autor oryginalnego projektu [ESP32 Marauder](https://github.com/justcallmekoko/ESP32Marauder).
