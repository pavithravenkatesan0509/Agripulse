# AgriGuard – Automated Rain Protection and Solar-Powered Lighting System

## Overview
AgriGuard is a smart-agriculture concept that combines rainfall detection, a motor-driven protective sheet, solar energy storage, and supplemental LED lighting. The goal is to reduce crop exposure to excessive rainfall and help provide light during prolonged cloudy or rainy periods.

## Problem
- Sudden or heavy rainfall can damage crops and contribute to waterlogging.
- Prolonged cloudy weather can reduce natural sunlight available to crops.
- Manual covering of crops can take time and labour.

## Proposed approach
1. A rain sensor (FC-37 or YL-83) detects rainfall.
2. A microcontroller (Arduino Uno in the documented simulation; ESP32 is an option for future connectivity) reads the sensor.
3. When the configured rain threshold is reached, a servo/motor mechanism deploys the protective sheet.
4. Supplemental LED lighting is switched on during the rain/low-light condition described in the prototype.
5. A solar panel, charge controller, and battery are proposed to supply stored renewable energy.

## Repository contents
- `docs/system-design.md` — architecture and operating sequence.
- `docs/components-and-testing.md` — components and the test observations reported in the paper.
- `docs/source-content.md` — text extracted from the project presentation for reference.
- `paper/IEEE-Paper-Agriguard.pdf` — original IEEE-style project paper.
- `presentation/AgriGuard-Project-Presentation.pptx` — original project presentation.

## Current implementation status
The uploaded paper describes a prototype/simulation and reports a rain-sensor threshold of 400, a 2–5 second response time, and servo positions of 0° (open) and 90° (close). These are reported project values, not independently verified performance guarantees. The original materials do not provide a complete standalone source-code file, so this repository does not claim that a complete firmware implementation is included yet.

## Keywords
Smart agriculture, rain sensor, crop protection, protective sheet, Arduino Uno, servo motor, solar power, LED lighting.
