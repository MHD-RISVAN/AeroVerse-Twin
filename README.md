# RC Boeing 737-900

**Project:** Scale RC model of Boeing 737-900 (max)

**Owner:** Mhd Risvan

---

## Project Overview

This repository documents the design, parts, electronics, and build notes for a 1:42 scale RC model of a Boeing 737-900. The aim is to build a flyable, scale-looking model approximately 100 cm long with retractable (or semi-retractable) landing gear, working flaps, lights, and reliable twin-motor propulsion.

---

## Research Notes

```
Boeing 737-900

length = 100 cm
actual dimension:
Real fuselage length ≈ 42 m = 4200 cm
Real wingspan ≈ 36 m = 3600 cm
Real fuselage diameter ≈ 3.76 m = 376 cm

model Scale: Scale = 100 / 4200 = 1/42 (dimesion actual body) (1:42)

```

## Dimensions
| Part | Dimension | Note |
| :--- | :--- | :--- |
| **Fuselage length** | 100cm | fixed |
| **Wingspan** | 3600/42=85.7cm | end to end length |
| **Fuselage diameter** | 376/42=8.95cm | |
| **Wing root chord** | ~660/42=15.7cm | longest width of the wings |
| **Wing tip chord** | ~160/42=3.8cm | width at the wing tip |
| **Horizontal tail span** | ~1230/42=29.3cm | length of horizontal stabilizer |
| **Vertical tail height** | ~880/42=21.0cm | vertical stabilizer |

(reference only, I have the exact scale, plan) image:

```

Assumption:
Comfortable thrust = 1.3× weight (help me to recover from bad flight and launch)


ground clearance (beneath the engine):
real Boeing 747-900 -> 48 cm
Scaled clearance (our model)= 1.1 cm  [1:42]

verdict:
we might need to use longer landing gear + shorter propeller.

propeller: (6 × 4 inch)
6 inch propeller
geometry:- 6-inch prop diameter = 15.24 cm -> Prop radius = 7.62 cm
6 × 4 inch

verdict:
we can't use high 8, 9, or 10 inch propellers to be more efficient, due to the ground clearance. Even though our choice is power hungry.

Brushless motor:
DYS D2830-11 1000KV

LiPo Batter: (3000 - 3500 ₹)
3S, 3000–4000 mAh (11.1 V)
capacity -> 30C or higher
XT60 connector

ESC:
40A per ESC
3S (11.1V) supportable
BEC:- 5V and ≥3A

servo motor:
SP Electron 4.8V- 6V MG90 Metal Gear Digital Servo Motor (https://amzn.to/4sceRbT)
Elevator	1	
Ailerons	2(One per wing)
Rudder	1
Nose-wheel steering	1
flap           2
extension and retraction servo    3 or 2 (if possible)

transmitter and receiver:
Radiolink T8FB 2.4GHz 8 Channels RC Remote Transmitter with R8EF Receiver, Dual Stick Controller (https://amzn.to/4qxq1GB)
```

---

## Parts List (derived from research)

> All items below match the detailed research above.

* **Airframe**: Foam / balsa / composite as planned — final fuselage length: **100 cm**
* **Motors (x2)**: DYS D2830-11 1000KV
* **Propellers**: 6 × 4 inch (electric, 2-blade) — consider 6×4.5 if temps allow
* **Battery**: 3S LiPo, **3000–4000 mAh**, **≥30C**, **XT60** connector (priced ~3000–3500 INR)
* **ESCs (x2)**: **40A** airplane ESC, 2–4S support, with **5V ≥ 3A BEC** (use one BEC only)
* **Servos**:

  * Elevator: 1 × MG90 (metal gear) or equivalent (≥2.5 kg·cm)
  * Ailerons: 2 × MG90 (one per wing)
  * Rudder: 1 × MG90
  * Nose-wheel steering: 1 × MG90 (metal recommended)
  * Flaps: 1–2 × MG90
  * Retract servos (if using servo retracts): 2–3 × high-torque servos (≥5 kg·cm) or dedicated retract actuators
* **Radio**: Radiolink T8FB transmitter + **R8EF** receiver (8 channels)

---

## Dial ESC with BEC - Note

* Use **two ESCs**, one per motor; **disable BEC on second ESC** (remove red wire) to avoid BEC conflicts.

---

## Landing Gear Options & Notes

* Options:

  * **Fixed gear** Easy and Cheap
  * **Servo-driven retracts** using high-torque servos
  * **Electric retract units** Great performance with easy installation in a small space.(best but expensive)

* Challenges:
  
  * The **landing gear** will be slightly longer to achieve the required ground clearance, due to the motor and propeller radius.
  * **Full retraction** is difficult because of the limited internal space in the model.
  * **Partial retract (semi-exposed wheels)** helps reduce drag and is easier to implement within the available space.


* needed to use higher torque servos such as MG995/MG996R or a dedicated one.

---

## Flight and Safety Notes

* Target All-Up Weight (AUW): **≤ 1.3 kg** to keep thrust-to-weight and runway requirements safe.
* Centre of Gravity

---

**End of README**

