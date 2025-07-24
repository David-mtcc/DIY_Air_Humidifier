# 💧 DIY Air Humidifier
This project is a simple **humidity-based controller** for a 5V ultrasonic humidifier, using an **Arduino Nano**, **DHT11 sensor**, **potentiometer**, **NPN transistor**, and a **TM1637 4-digit display**.

When the **humidity drops below a user-defined setpoint**, the system automatically powers on the humidifier. The setpoint is adjusted via a potentiometer, and both the setpoint and current humidity are shown on the display.

---

## 🧰 Components Used

- Arduino Nano (Rev3.0)
- DHT11 Humidity & Temperature Sensor
- 10kΩ Potentiometer or Trimmer
- TM1637 4-digit 7-segment display
- NPN transistor (e.g. 2N2222 or S8050)
- 220Ω resistors (×2)
- Red LED (used as an activity indicator)
- [5V ultrasonic atomizer](https://www.amazon.de/-/en/Atomiser-Humidifier-Atomization-Integrated-Circuit/dp/B0946L91HL)
- Breadboard & jumper wires
- Power source (USB or 5V supply)

---

## 📐 Circuit Overview

- The **DHT11** measures ambient humidity.
- The **potentiometer** sets the desired humidity setpoint (30%–70%).
- A **TM1637 display** shows:
  - First two digits: setpoint (e.g. `45`)
  - Last two digits: current humidity (e.g. `38`)
- An **NPN transistor** switches on the **LED and humidifier** when humidity is below the setpoint.
- Everything is powered at **5V**, and controlled by the **Arduino Nano**.

---

## 💾 Libraries Required

Install via the **Arduino Library Manager**:

- [`DHT sensor library`](https://github.com/adafruit/DHT-sensor-library)
- [`TM1637Display`](https://github.com/avishorp/TM1637)

---

## 📟 Display Output

Setpoint: 45%
Humidity: 38%
Display: 4538

When the humidity drops below the setpoint, the **transistor activates**, powering the **LED and humidifier**.

---

## 📸 Project Preview
Note: instead of the led, a 5V ultrasonic atomizer must be used.

![Humidifier_bb](https://github.com/user-attachments/assets/4a53ee18-dd36-4d25-89b3-8075b9fe159c)

