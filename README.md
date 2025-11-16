# BL917-Solar-Charger-Controller
Monitor and control your BL917 MPPT solar controller from your phone
![image]((https://github.com/swedenfox/BL917-Solar-Charger-Controller/assets/readme/bl917solarcontroller.jpg)

A cross platform Flutter app that connects to the BL917 MPPT solar charge controller using its hidden WebSocket API.  
No registration, no vendor cloud, full local control.

Developed by **Andrea Nostro**.

## Features

- Direct WebSocket connection to `ws://device.gz529.com`
- MAC address input plus Bluetooth scan for nearby ZJBX devices
- Real time dashboard with dynamic icons:
  - Sun / moon depending on charging state
  - Battery with or without lightning bolt while charging
  - Light bulb on or off depending on load state
- Live monitoring of:
  - Battery voltage, temperature, charge and discharge current
  - Load state and estimated load power
  - Total power generation (kWh)
- Energy savings estimation based on:
  - User configurable cost per kWh
  - User selected currency
- Settings page for:
  - Float, cutoff and restore voltages
  - Load working hours
  - Battery type
- Device page for:
  - Charge mode control (manual, auto, timing, straight out)
  - Load on or off
  - Raw properties list for debugging

## Tech stack

- Flutter
- Dart
- WebSocket communication
- `flutter_blue_plus` for Bluetooth scanning


