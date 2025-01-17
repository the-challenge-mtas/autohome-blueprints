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

[![Import Blueprint](https://my.home-assistant.io/badges/blueprint_import.svg)](https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https%3A%2F%2Fgithub.com%2Fthe-challenge-mtas%2Fautohome-blueprints%2Fblob%2Fmaster%2Flighting%2Fadaptive-lighting.yaml)

**Trigger:**

- Motion detected by the PIR sensor or presence detected by the mmWave sensor.
- Lux sensor reports low light levels.

**Conditions:**

- Time of day is evening or night.
- No recent motion or presence activity (e.g., after 15 minutes of inactivity, turn off the light).

**Action:**

- Turn on lights to the previous brightness level when the lux reading is under the threshold.

---

### Lighting Based on Presence

[![Import Blueprint](https://my.home-assistant.io/badges/blueprint_import.svg)](https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https%3A%2F%2Fgithub.com%2Fthe-challenge-mtas%2Fautohome-blueprints%2Fblob%2Fmaster%2Flighting%2FmmWave-presence-lighting.yaml)

**Trigger:**

- Presence detected by the mmWave sensor.

**Conditions:**

- No recent presence (e.g., after 15 minutes of inactivity, turn off the light).

**Action:**

- Turn on lights to the previous brightness level when presence is detected.

---

### Thermostat Adjustment Based on Room Occupancy

[![Import Blueprint](https://my.home-assistant.io/badges/blueprint_import.svg)](https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https%3A%2F%2Fgithub.com%2Fthe-challenge-mtas%2Fautohome-blueprints%2Fblob%2Fmaster%2Ftemperature%2Foccupancy-thermostat.yaml)

**Trigger:**

- Door contact sensor changes to "open" or "closed."
- mmWave sensor detects presence.

**Conditions:**

- Temperature reading from the thermometer is below or above a set threshold.

**Action:**

- Adjust the thermostat settings to maintain comfort when the room is occupied.

---

### Pause Music When Room is Empty

[![Import Blueprint](https://my.home-assistant.io/badges/blueprint_import.svg)](https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https%3A%2F%2Fgithub.com%2Fthe-challenge-mtas%2Fautohome-blueprints%2Fblob%2Fmaster%2Fmedia%2Fplayback-stop.yaml)

**Trigger:**

- Motion sensor detects no motion.
- Presence sensor detects no presence.

**Conditions:**

- Specified duration of inactivity has passed.

**Action:**

- Pause the media player if no motion or presence is detected.

## Contributing

We welcome contributions! If you have a blueprint that you would like to share, please submit a pull request.

## Contact

For any questions or suggestions, please open an issue or contact us directly.

Happy automating with AutoHome!
