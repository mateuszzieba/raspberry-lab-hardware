# **Dokumentacja Raspberry Pi – Podstawowe Informacje**

---

## **Schemat Pinów GPIO (40-pinowy header)**

| Pin | Funkcja            | Pin | Funkcja            |
|-----|--------------------|-----|--------------------|
| 1   | 3.3V              | 2   | 5V                 |
| 3   | GPIO2 (SDA, I2C)  | 4   | 5V                 |
| 5   | GPIO3 (SCL, I2C)  | 6   | GND                |
| 7   | GPIO4             | 8   | GPIO14 (UART TXD)  |
| 9   | GND               | 10  | GPIO15 (UART RXD)  |
| 11  | GPIO17            | 12  | GPIO18 (PWM)       |
| 13  | GPIO27            | 14  | GND                |
| 15  | GPIO22            | 16  | GPIO23             |
| 17  | 3.3V              | 18  | GPIO24             |
| 19  | GPIO10 (SPI MOSI) | 20  | GND                |
| 21  | GPIO9 (SPI MISO)  | 22  | GPIO25             |
| 23  | GPIO11 (SPI SCLK) | 24  | GPIO8 (SPI CE0)    |
| 25  | GND               | 26  | GPIO7 (SPI CE1)    |
| 27  | ID_SD (I2C ID)    | 28  | ID_SC (I2C ID)     |
| 29  | GPIO5             | 30  | GND                |
| 31  | GPIO6             | 32  | GPIO12 (PWM)       |
| 33  | GPIO13 (PWM)      | 34  | GND                |
| 35  | GPIO19 (PWM)      | 36  | GPIO16             |
| 37  | GPIO26            | 38  | GPIO20             |
| 39  | GND               | 40  | GPIO21             |

---

## **Opis Pinów GPIO**

### **1. Zasilanie**
- **3.3V (Pin 1, Pin 17)**: Zasilanie urządzeń peryferyjnych (czujniki, moduły).
- **5V (Pin 2, Pin 4)**: Bezpośrednie zasilanie z Raspberry Pi.
- **GND (Pin 6, 9, 14, 20, 25, 30, 34, 39)**: Masa (wspólny punkt odniesienia).

### **2. Interfejs I2C**
- **SDA (Pin 3, GPIO2)**: Linie danych.
- **SCL (Pin 5, GPIO3)**: Zegar I2C.

### **3. Interfejs SPI**
- **MOSI (Pin 19, GPIO10)**: Master Out Slave In (dane do urządzenia).
- **MISO (Pin 21, GPIO9)**: Master In Slave Out (dane od urządzenia).
- **SCLK (Pin 23, GPIO11)**: Zegar SPI.
- **CE0 (Pin 24, GPIO8)**: Chip Select 0.
- **CE1 (Pin 26, GPIO7)**: Chip Select 1.

### **4. Interfejs UART**
- **TXD (Pin 8, GPIO14)**: Transmisja danych.
- **RXD (Pin 10, GPIO15)**: Odbiór danych.

### **5. Ogólne GPIO**
- Dowolne piny GPIO (np. GPIO17, GPIO18) mogą być skonfigurowane jako wejścia lub wyjścia cyfrowe w zależności od Twojego projektu.

### **6. PWM**
- **GPIO18 (Pin 12), GPIO13 (Pin 33), GPIO19 (Pin 35)**: Wyjście PWM (modulacja szerokości impulsu) do sterowania np. serwomechanizmami.

---

## **Przydatne Linki i Dokumentacja**

1. Oficjalna strona Raspberry Pi:  
   [https://www.raspberrypi.org](https://www.raspberrypi.org)

2. Dokumentacja GPIO:  
   [https://pinout.xyz](https://pinout.xyz)

3. Kompendium o Raspberry Pi:  
   [https://www.raspberrypi.org/documentation](https://www.raspberrypi.org/documentation)

4. Dokumentacja Python dla Raspberry Pi (biblioteka `RPi.GPIO`):  
   [https://sourceforge.net/p/raspberry-gpio-python/wiki/Home/](https://sourceforge.net/p/raspberry-gpio-python/wiki/Home/)

5. Przykładowe projekty i tutoriale:  
   [https://projects.raspberrypi.org/en](https://projects.raspberrypi.org/en)
