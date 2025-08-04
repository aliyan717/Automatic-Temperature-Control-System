# 🔥 Automatic Temperature Control System

This project is an Arduino-based system that automatically controls the speed of a DC fan using a 10k NTC thermistor. It is capable of adjusting fan speed based on temperature, with user-configurable limits, and includes features like real-time LCD display and a buzzer alarm for over-temperature warning.

## 📘 Project Overview

This project demonstrates how a microcontroller (Arduino UNO) can be used to monitor and control temperature within a system. The core functionality includes:

- Reading temperature using an NTC Thermistor
- Adjusting fan speed using PWM and a power MOSFET (IRFZ44N)
- Allowing the user to set upper and lower temperature thresholds
- Displaying real-time information on a 16x2 LCD
- Triggering a buzzer alarm if the temperature exceeds the upper limit

---

## 🧰 Components Used

| Component           | Description                                   |
|--------------------|-----------------------------------------------|
| Arduino UNO        | Main microcontroller                          |
| NTC Thermistor 10k | Senses temperature based on resistance        |
| IRFZ44N MOSFET     | Controls the fan speed                        |
| 16x2 LCD           | Displays temperature and fan status           |
| Buzzer             | Audible alert for over-temperature            |
| Push Buttons       | For setting temperature limits                |
| DC Fan             | Cooling component                             |
| Potentiometer      | Adjusts LCD contrast                          |

---

## 🛠️ How It Works

1. The system constantly reads temperature using the thermistor.
2. It calculates the exact temperature using the Steinhart-Hart equation.
3. If temperature > set limit, the fan activates using PWM through the MOSFET.
4. A buzzer sounds if the temperature exceeds the maximum threshold.
5. The user can set temperature ranges using the push buttons.

---

## 📊 Simulation

This project was simulated using **Proteus**. The circuit includes:

- Thermistor input
- LCD interface
- PWM-controlled fan via IRFZ44N
- EEPROM-based memory for saving threshold settings

---

## 📷 Screenshots / Circuit Diagram

You can add images here using:

```markdown
(circuit.png)
