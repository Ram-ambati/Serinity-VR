# Serenity VR 🧘‍♂️🥽

> An AI-driven, biofeedback-adapted Virtual Reality therapy system for anxiety management.

**Short Description for GitHub:** A closed-loop VR therapy platform that uses real-time SpO2 and heart rate data (MAX30102 + ESP32) to dynamically adapt Unity VR scenes via a local AI agent (Ollama) and Spring Boot backend.

## Recommended GitHub Tags
`virtual-reality`, `biofeedback`, `anxiety-therapy`, `esp32`, `max30102`, `spring-boot`, `react`, `unity3d`, `ollama`, `local-ai`, `health-tech`

## Project Structure

This repository is a monorepo containing all components of the Serenity VR system:

- 📁 **[`serenity-backend/`](./serenity-backend/)** - Spring Boot application handling MQTT, WebSockets, and AI orchestration.
- 📁 **[`serenity-dashboard/`](./serenity-dashboard/)** - React clinician dashboard for live biometric monitoring.
- 📁 **[`serenity-hardware/`](./serenity-hardware/)** - ESP32 firmware (C++) for reading MAX30102 sensor data and publishing via MQTT.
- 📁 **[`serenity-vr/`](./serenity-vr/)** - Unity project containing adaptive therapeutic VR scenes (Meta Quest).
- 📁 **[`Docs/`](./Docs/)** - Documentation, system architecture, systems mapping (Iceberg/CLD), and feasibility studies.

## Architecture Overview
*(See `Docs/` for full details)*
1. Patient wears the MAX30102 sensor connected to an ESP32.
2. ESP32 transmits SpO2 and Heart Rate data via MQTT to the Spring Boot backend.
3. The backend consults a local Llama 3 AI model for real-time therapeutic adaptations.
4. The backend streams adaptive commands via WebSocket to the Unity VR headset.
5. Clinicians can monitor the session live via the React dashboard.
