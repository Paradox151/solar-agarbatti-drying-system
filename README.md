# Solar-Powered Agarbatti Drying & Packaging System

A compact drying and packaging system designed for home-based
agarbatti manufacturing by rural women artisans.

## 🏆 Hackathon

Smart India Hackathon 2026

Problem Statement: SIH26022

## 📌 Overview

The project aims to improve the drying and packaging workflow of
home-based agarbatti manufacturing through controlled heating,
airflow, sensing and weight-based packaging.

## 🎯 Problem

Traditional drying methods can depend heavily on environmental
conditions and may result in inconsistent drying.

This system explores a controlled drying chamber with temperature
and humidity monitoring.

## ⚙️ System Architecture

The drying chamber consists of:

- Heating element
- Fan-assisted airflow
- Two drying trays
- Air diffuser/plenum
- Temperature sensors
- Humidity sensor
- ESP32 controller
- Safety cutoff system

## 🔧 Hardware

- ESP32
- DS18B20 × 2
- DHT22
- Heating coil
- 12V DC fan
- Relay/MOSFET
- Thermal fuse
- Aluminum chamber
- Aluminum mesh trays
- Load cell
- HX711 amplifier
- LCD/OLED display

## 🧠 Control Logic

The controller operates using a state-machine architecture:

IDLE
↓
HEATING
↓
MAINTAINING
↓
COMPLETE

A separate FAULT state handles abnormal temperature conditions.

## 📦 Packaging System

The packaging station uses a load cell and HX711 amplifier
for weight-based portioning.

Basic workflow:

1. Place empty bag on load cell
2. Tare the scale
3. Add agarbatti sticks
4. Monitor weight
5. Signal when target weight is reached
6. Remove and manually seal the packet

## 🛡️ Safety

The design incorporates multiple safety layers:

- Software temperature control
- Independent firmware overheat cutoff
- Physical thermal fuse

## 🔋 Power

The concept uses solar PV and battery power as the intended
primary power system, with grid power as backup.

The prototype currently uses available hardware for MVP
demonstration.

## 📊 MVP Status

Current prototype focuses on validating:

- Controlled drying
- Temperature monitoring
- Humidity monitoring
- Airflow
- Weight-based packaging
- Safety mechanisms

## 🚧 Future Improvements

- Automated bag dispensing
- Automated sealing
- Conveyor/feeding mechanism
- Label/date printing
- Battery-backed solar operation
- IoT monitoring and alerts

## 👥 Team

Team project developed for Smart India Hackathon 2026.

**My Role:** Team Member

## 📷 Prototype

![Prototype](prototype.jpg)
