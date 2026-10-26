# AgriGuard System Design

## Purpose
Protect crops from excessive rainfall using a sensor-triggered cover and provide supplemental artificial lighting during rainy or low-sunlight periods.

## Main modules
- **Rain detection unit:** FC-37/YL-83 rain sensor detects water on its sensing surface.
- **Control unit:** Arduino Uno reads the analog sensor value and decides whether to activate the mechanism.
- **Protective-sheet actuation:** Servo/motor mechanism deploys or retracts the cover.
- **Lighting unit:** LED lighting is controlled to provide supplemental light in the described rain condition.
- **Power unit:** Solar panel, charge controller, and battery are proposed to collect and store energy for the system.

## Operating sequence
1. Continuously read the rain sensor.
2. Compare the sensor reading with the configured threshold.
3. If rain is detected, move the actuator to the cover position and turn on the LED indicator/light.
4. If rain is not detected, return the actuator to its normal position and turn the LED off.
5. Repeat the monitoring cycle.

## High-level flowchart
```text
Start
  |
Initialize sensor, servo/motor and LED
  |
Read rain sensor
  |
Is rain detected?
  | Yes                 | No
Deploy protective       Retract/keep cover
sheet                   in normal position
Turn LED on             Turn LED off
  |                       |
  +------ Read sensor again ------+
```

## Important implementation note
The paper describes an Arduino-based simulation and also discusses solar-powered operation. The exact wiring, motor-driver arrangement, battery sizing, and solar charge-control design must be finalized and tested for the actual hardware before field deployment.
