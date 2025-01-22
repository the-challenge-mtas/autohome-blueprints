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

### Adaptive Lighting Based on PIR Sensor

[![Import Blueprint](https://my.home-assistant.io/badges/blueprint_import.svg)](https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https%3A%2F%2Fgithub.com%2Fthe-challenge-mtas%2Fautohome-blueprints%2Fblob%2Fmaster%2Flighting%2Fadaptive-lighting-PIR.yaml)

**Trigger:**

- Motion detected by the PIR sensor.

**Action:**

- Turn on lights when motion is detected.
- Turn off lights after a specified period of inactivity.

---

### Adaptive Lighting Based on PIR Sensor and Lux

[![Import Blueprint](https://my.home-assistant.io/badges/blueprint_import.svg)](https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https%3A%2F%2Fgithub.com%2Fthe-challenge-mtas%2Fautohome-blueprints%2Fblob%2Fmaster%2Flighting%2Fadaptive-lighting-PIR-min-lux.yaml)

**Trigger:**

- Motion detected by the PIR sensor.

**Conditions:**

- Lux sensor reports low light levels.

**Action:**

- Turn on lights when motion is detected and light levels are low.
- Turn off lights after a specified period of inactivity.

---

### Adaptive Lighting Based on mmWave Sensor

[![Import Blueprint](https://my.home-assistant.io/badges/blueprint_import.svg)](https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https%3A%2F%2Fgithub.com%2Fthe-challenge-mtas%2Fautohome-blueprints%2Fblob%2Fmaster%2Flighting%2Fadaptive-lighting-mmWave.yaml)

**Trigger:**

- Presence detected by the mmWave sensor.

**Action:**

- Turn on lights when presence is detected.
- Turn off lights after a specified period of inactivity.

---

### Adaptive Lighting Based on mmWave Sensor and Lux

[![Import Blueprint](https://my.home-assistant.io/badges/blueprint_import.svg)](https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https%3A%2F%2Fgithub.com%2Fthe-challenge-mtas%2Fautohome-blueprints%2Fblob%2Fmaster%2Flighting%2Fadaptive-lighting-mmWave-min-lux.yaml)

**Trigger:**

- Presence detected by the mmWave sensor.

**Conditions:**

- Lux sensor reports low light levels.

**Action:**

- Turn on lights when presence is detected and light levels are low.
- Turn off lights after a specified period of inactivity.

---

### Radar-activated Light

[![Import Blueprint](https://my.home-assistant.io/badges/blueprint_import.svg)](https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https%3A%2F%2Fgithub.com%2Fthe-challenge-mtas%2Fautohome-blueprints%2Fblob%2Fmaster%2Flighting%2FmmWave-presence-lighting.yaml)

**Trigger:**

- Presence detected by the mmWave sensor.

**Action:**

- Turn on lights when presence is detected.
- Turn off lights after a specified period of inactivity.

---

### Pause Music When Room is Empty (PIR Sensor)

[![Import Blueprint](https://my.home-assistant.io/badges/blueprint_import.svg)](https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https%3A%2F%2Fgithub.com%2Fthe-challenge-mtas%2Fautohome-blueprints%2Fblob%2Fmaster%2Fmedia%2Fplayback-stop-pir.yaml)

**Trigger:**

- Motion sensor detects no motion.

**Conditions:**

- Specified duration of inactivity has passed.

**Action:**

- Pause the media player if no motion is detected.

---

### Pause Music When Room is Empty (mmWave Sensor)

[![Import Blueprint](https://my.home-assistant.io/badges/blueprint_import.svg)](https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https%3A%2F%2Fgithub.com%2Fthe-challenge-mtas%2Fautohome-blueprints%2Fblob%2Fmaster%2Fmedia%2Fplayback-stop-mmwave.yaml)

**Trigger:**

- Presence sensor detects no presence.

**Conditions:**

- Specified duration of inactivity has passed.

**Action:**

- Pause the media player if no presence is detected.

---

### Lower Thermostat When Window Opened

[![Import Blueprint](https://my.home-assistant.io/badges/blueprint_import.svg)](https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https%3A%2F%2Fgithub.com%2Fthe-challenge-mtas%2Fautohome-blueprints%2Fblob%2Fmaster%2Ftemperature%2Fcontact-ecomode-thermostat.yaml)

**Trigger:**

- Window contact sensor detects the window is open.

**Action:**

- Lower the thermostat temperature when the window is open.

---

### Lower Thermostat When No Presence Detected (mmWave)

[![Import Blueprint](https://my.home-assistant.io/badges/blueprint_import.svg)](https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https%3A%2F%2Fgithub.com%2Fthe-challenge-mtas%2Fautohome-blueprints%2Fblob%2Fmaster%2Ftemperature%2FmmWave-ecomode-thermostat.yaml)

**Trigger:**

- No presence detected by the mmWave sensor.

**Action:**

- Lower the thermostat temperature when no presence is detected.

---

### Lower Thermostat When No Motion Detected (PIR)

[![Import Blueprint](https://my.home-assistant.io/badges/blueprint_import.svg)](https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https%3A%2F%2Fgithub.com%2Fthe-challenge-mtas%2Fautohome-blueprints%2Fblob%2Fmaster%2Ftemperature%2FPIR-ecomode-thermostat.yaml)

**Trigger:**

- No motion detected by the PIR sensor.

**Action:**

- Lower the thermostat temperature when no motion is detected.

---

### Thermostat Adjustment Based on PIR Motion Sensor

[![Import Blueprint](https://my.home-assistant.io/badges/blueprint_import.svg)](https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https%3A%2F%2Fgithub.com%2Fthe-challenge-mtas%2Fautohome-blueprints%2Fblob%2Fmaster%2Ftemperature%2FPIR-thermostat.yaml)

**Trigger:**

- Motion detected by the PIR sensor.

**Conditions:**

- Temperature is below the specified threshold.

**Action:**

- Adjust the thermostat to the specified temperature.

---

### Thermostat Adjustment Based on Room Occupancy

[![Import Blueprint](https://my.home-assistant.io/badges/blueprint_import.svg)](https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https%3A%2F%2Fgithub.com%2Fthe-challenge-mtas%2Fautohome-blueprints%2Fblob%2Fmaster%2Ftemperature%2FmmWave-thermostat.yaml)

**Trigger:**

- Presence detected by the mmWave sensor.

**Conditions:**

- Temperature is below the specified threshold.

**Action:**

- Adjust the thermostat to the specified temperature.

## Contributing

We welcome contributions! If you have a blueprint that you would like to share, please submit a pull request.

## Contact

For any questions or suggestions, please open an issue or contact us directly.

Happy automating with AutoHome!
