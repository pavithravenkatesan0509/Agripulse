# Components and Testing Notes

## Components mentioned in the project materials
| Component | Purpose |
|---|---|
| FC-37 / YL-83 rain sensor | Detect rainfall |
| Arduino Uno | Read sensor values and control the prototype |
| Servo motor / motor arrangement | Deploy or retract the protective sheet |
| Waterproof protective sheet | Shield crops from direct rainfall |
| LED light | Supplemental lighting during rainy/low-sunlight conditions |
| Solar panel | Generate renewable energy |
| Battery and charge controller | Store and regulate solar energy |

## Values reported in the IEEE-style paper
| Parameter | Reported value / observation |
|---|---|
| Rain detection method | Analog sensor input (A0) |
| Threshold | 400 |
| Response time | 2–5 seconds |
| Servo action | 0° (open), 90° (close) |
| LED operation | ON during rain, OFF when no rain |
| System operation | Automatic |
| Power source | Solar panel + battery |

The paper also reports detection accuracy of 95% and system reliability of 92%. These are values stated in the supplied paper; the repository does not independently validate them.

## Testing checklist for a physical prototype
- Test sensor readings with dry and wet sensor surfaces.
- Adjust the threshold using actual sensor readings.
- Confirm that the protective sheet opens and closes without jamming.
- Confirm the LED switching behaviour.
- Check power consumption and battery capacity under realistic conditions.
- Test manual override and safe stopping before field use.
