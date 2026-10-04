# AquaGuard – Real-Time Water Leakage Monitoring System

AquaGuard is an ESP32-based IoT water leakage monitoring system designed to detect critical water loss by continuously comparing the flow rate at the inlet and outlet of a pipeline.

The system uses two YF-S201 water flow sensors to monitor water flow, an ESP32 for processing, a 16×2 I2C LCD for local monitoring, and Blynk IoT for remote monitoring. During a critical leakage condition, the system activates a red LED, sounds an active buzzer, and closes the solenoid valve through a relay module.

---

## Features

- Real-time monitoring of inlet and outlet water flow
- Dual YF-S201 water flow sensors
- ESP32-based flow processing and leak detection
- 16×2 I2C LCD for local display
- Blynk IoT dashboard for remote monitoring
- Yellow LED indication for normal operation
- Red LED indication for critical leakage
- Active buzzer for critical leakage alert
- Relay-controlled solenoid valve for automatic shut-off
- Physical reset button
- Blynk app reset control
- Blynk leak notification
- Flow averaging for more stable measurements

---

## Working Principle

AquaGuard measures the water flow at two points in the pipeline:

```text
Water In
   │
   ▼
Flow Sensor 1
(INLET)
   │
   ▼
Pipeline / Leak Point
   │
   ▼
Solenoid Valve
   │
   ▼
Flow Sensor 2
(OUTLET)
   │
   ▼
Water Out
