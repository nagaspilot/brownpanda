# brownpanda

**Automotive Gateway Hardware for Universal ADAS Integration**

brownpanda is NagasPilot's specialized automotive gateway hardware that enables universal vehicle compatibility while maintaining the highest safety standards.

## Overview

brownpanda translates between vehicle-specific protocols and a universal Tesla Model 3 standard CAN bus protocol (500 kbps, non-CAN-FD), enabling openpilot compatibility across any vehicle brand.

## Architecture

### Hardware Specifications
- **Safety Grade**: AEC-Q100 automotive qualification
- **Microcontroller**: Automotive-grade with fail-safe fallback mechanisms
- **Protocol Support**: Universal vehicle protocol translation
- **Safety Features**: Physical override switch with instant deactivation

### Protocol Standard
- **Base Protocol**: Tesla Model 3 CAN bus (500 kbps, non-CAN-FD)
- **Compatibility**: Comma 3 classic and newer devices
- **Translation**: Bidirectional vehicle protocol ↔ Tesla protocol conversion

## Safety Features

### Hardware Safety
- AEC-Q100 grade automotive microcontrollers
- Fail-safe fallback mechanisms
- Hardware watchdog and redundancy systems

### User Safety
- **Physical Switch**: Instant system override capability
- **OEM ADAS Preservation**: Factory ADAS remains functional when switch is not engaged
- **Seamless Mode Switching**: In enhancedpilot, ADAS safety logic migrates to brownpanda for smooth OEM ↔ enhancedpilot transitions

## enhancedpilot Integration

For the enhancedpilot project, brownpanda provides enhanced capabilities:

- **Safety Logic Migration**: ADAS safety moved to gateway hardware
- **Mode Switching**: Seamless integration between OEM ADAS and enhancedpilot
- **Hardware Arbitration**: Intelligent control handoff between systems
- **Fallback Protection**: Automatic return to OEM ADAS on any fault condition

## Technical Specifications

### Communication
- **Primary CAN**: 500 kbps standard CAN bus
- **Vehicle CAN**: Varies by vehicle (translated by brownpanda)
- **Diagnostic**: OBD-II pass-through support
- **Update Interface**: Secure firmware update capability

### Power Requirements
- **Operating Voltage**: 12V automotive (9-16V tolerance)
- **Power Consumption**: <5W typical operation
- **Standby Current**: <50mA when vehicle off

### Environmental
- **Operating Temperature**: -40°C to +85°C
- **Storage Temperature**: -55°C to +125°C
- **Vibration**: Automotive grade (ISO 16750-3)
- **EMI/EMC**: Meets automotive standards

## Development Status

brownpanda is currently in active development for Chinese EV market integration.

### Current Status
- ✅ Core protocol translation engine
- ✅ Safety watchdog implementation
- ✅ Physical override switch
- 🔄 Vehicle-specific tuning profiles
- 🔄 OEM ADAS integration testing

### Roadmap
- Enhanced sensor fusion support (radar, LiDAR)
- Extended vehicle protocol library
- Advanced diagnostic capabilities
- Over-the-air update system

## Safety & Compliance

⚠️ **IMPORTANT SAFETY NOTICE**

brownpanda is automotive safety-critical hardware. Improper installation or modification can result in:
- Loss of vehicle control
- Unexpected acceleration/braking
- Safety system failures

**Requirements:**
- Professional installation recommended
- Proper wiring and grounding essential
- Regular safety validation testing
- Compliance with local vehicle modification laws

## Community

We do not have a dedicated Discord or Slack channel. For discussions and community support, visit our Facebook page:

- **Facebook**: [https://www.facebook.com/nagaspilot](https://www.facebook.com/nagaspilot)

## License

brownpanda hardware design and firmware are proprietary to NagasPilot.

Software integration libraries are MIT licensed where applicable.

---

**THIS IS ALPHA QUALITY HARDWARE FOR RESEARCH PURPOSES ONLY. THIS IS NOT A PRODUCT.
YOU ARE RESPONSIBLE FOR COMPLYING WITH LOCAL LAWS AND REGULATIONS.
NO WARRANTY EXPRESSED OR IMPLIED.**

## Community

We do not have a dedicated Discord or Slack channel. For discussions and community support, visit our Facebook page:

- **Facebook**: [https://www.facebook.com/nagaspilot](https://www.facebook.com/nagaspilot)
