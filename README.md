# ESP32 heating valve controller

This projects is about an ESP32 based heating valve controller using Homematic IP actors to control heating valves,
usually for floorboard heating.

## ESPHOME

Included in this repository are esphome configs for controlling the motors.
Include them with the following lines in your esphome config yml:

```
packages:
  valve_controller_2_0:
    url: https://github.com/lal12/esp-valve-controller
    ref: master
    file: esphome/v2.0.yml
    refresh: 1d # optional
    vars:
      LED_INTERNAL: false
  valve_controller_1_0:
    url: https://github.com/lal12/esp-valve-controller
    ref: master
    file: esphome/v1.0.yml
    refresh: 1d # optional
```
