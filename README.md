# kegcleaner - ESPHome project for Kincony A16 board

Kegcleaner is automation of KEG sanitizing machine used in small breweries. It uses Kincony A16 board with some SSR relay for control of a few solenoid valves and contactors.


## Input mediums - controlled by solenoid valves
- Water
- Hot Water
- Clean Air (high pressure)
- Reduced Air (2 bar clean air)
- Innert Gas (CO2 or N)

## Input mediums which is controlled by pump
- Sanitizing Solution (2-3% NaOH or some Acidic Solution) in tank

## Output Solenoids Valves
- Drain
- Return into solution tank

Output Solenoids can't be opened together.

##  Thermostat (Climate control)
- DS18B20 temperature sensor
- 3-phase contator for heating spiral

## Automation Process

Automation process includes:
- Emptying KEG
- Pre-clean with hot water and reduced air
- Clean process
- Post-clean process
- Inflation KEG with innert gas

### TODOs
- Variable cleaning time according to size of KEG
- Variable post-cleaning lavage time
