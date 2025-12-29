# RC Boeing 737-900

**Project:** Scale RC model of Boeing 737-900 (max)

**Owner:** Mhd Risvan

---

## Project Overview

This repository documents the design, parts, electronics, and build notes for a 1:42 scale RC model of a Boeing 737-900. The aim is to build a flyable, scale-looking model approximately 100 cm long with retractable (or semi-retractable) landing gear, working flaps, lights, and reliable twin-motor propulsion.

---

## Research Notes (verbatim — do not remove)

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

> All items below match the detailed research above. Do not remove or alter the researched details.

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
* **Connectors & wiring**: XT60, bullet connectors, 14–16AWG power leads, heatshrink
* **Misc**: Battery strap, foam padding, servo horns, clevises, pushrods, control horns, pushrod guides

---

## Electronics & Power System Notes

* Use **two ESCs**, one per motor; **disable BEC on second ESC** (remove red wire) to avoid BEC conflicts.
* Calibrate both ESCs together with the TX before mounting props.
* Place ESCs and motors for airflow cooling; avoid burying ESCs in foam with no vents.
* Use **Y-lead** or radio mixing for dual-throttle control (one throttle channel from TX split to both ESCs) OR use radio mixing features carefully.

---

## Landing Gear Options & Notes

* You can choose between:

  * **Fixed gear** (cheapest and most reliable)
  * **Manual / mechanical retracts** (cheap, semi-automatic)
  * **Servo-driven retracts** using high-torque servos (~5–9 kg·cm)
  * **Electric retract units** (best but expensive)

* For scale look with budget, **partial retract (semi-exposed wheels)** is recommended: reduces drag, easier than full internal bays.

* If using servo-driven retracts, don’t use MG90 for retraction: use higher torque servos such as MG995/MG996R or a dedicated retract actuator.

---

## Flight and Safety Notes

* Target All-Up Weight (AUW): **≤ 1.3 kg** to keep thrust-to-weight and runway requirements safe.
* Aim for comfortable thrust ≈ **1.3× AUW** across both motors combined.
* Runway: use smooth tarmac or concrete; avoid grass for first flights.
* Pre-flight checklist: battery charged, ESCs calibrated, controls correct direction, CG checked, secure battery, props off during static checks.

---

## Build Plan (high level)

1. Finalize airframe structure and center of gravity (CG) location.
2. Mount motors, ESCs, servos, and receiver temporarily.
3. Place battery and test balance; aim CG at ~25–30% MAC.
4. Wire ESCs, calibrate throttles, test motor spin without props.
5. Install control linkages, check throws and directions, set end-points.
6. Ground test: taxi runs, motor heating, BEC load test.
7. Maiden flight from smooth runway, conservative trims and gentle rotation.

---

## Contribution & Notes for Hackclud

* This README is a living document — add measurement photos, flight logs, and incremental changes here.
* Preserve the original research block above as it contains important reference numbers used in layout and part selection.

---

## License

Add your preferred license here (MIT / CC BY‑SA suggested).

---

**End of README**
























## Key Features

## Planned Parts List (BOM)
| Part | Specification |
| :--- | :--- |
| **Radio** | FlySky FS-i6X / RadioLink T8FB |
| **Motors** | 2x 2212 1400KV Brushless |
| **ESC** | |
| **Battery** | 3S/4S LiPo |
| **Controller** | ESP32 (for data logging) |

## Related Projects
- [Lebrinex](https://lebrinex.vercel.app/) - Library Management System
- [Tilawanow](https://tilawanow.vercel.app/) - Quran Site
