# AutoHome Blueprints

Welcome to the AutoHome Blueprints repository! This repository contains a collection of blueprints designed to automate various aspects of your smart home.

## Getting Started

To use these blueprints, simply download the desired blueprint and import it into your AutoHome setup.

## Folder Structure

The blueprints are organized by the type of device they control:

- **Lighting**: Contains all light controlling automations.
- **Temperature**: Contains all thermostat controlling automations.
- **Media**: Contains all media controlling automations.

## Example Blueprints

### Adaptive Lighting Based on Motion, Lux, and Presence

[![Import Blueprint](https://my.home-assistant.io/badges/blueprint_import.svg)](https://my.home-assistant.io/redirect/blueprint_import/)

**Trigger:**

- Motion detected by the PIR sensor or presence detected by the mmWave sensor.
- Lux sensor reports low light levels.

**Conditions:**

- Time of day is evening or night.
- No recent motion or presence activity (e.g., after 15 minutes of inactivity, turn off the light).

**Action:**

- Turn on lights to a specific brightness level based on the lux reading.

---

### Thermostat Adjustment Based on Room Occupancy

[![Import Blueprint](https://my.home-assistant.io/badges/blueprint_import.svg)](https://my.home-assistant.io/redirect/blueprint_import/)

**Trigger:**

- Door contact sensor changes to "open" or "closed."
- mmWave sensor detects presence.

**Conditions:**

- Temperature reading from the thermometer is below or above a set threshold.

**Action:**

- Adjust the thermostat settings to maintain comfort when the room is occupied.

## Contributing

We welcome contributions! If you have a blueprint that you would like to share, please submit a pull request.

## Contact

For any questions or suggestions, please open an issue or contact us directly.

Happy automating with AutoHome!