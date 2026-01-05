# Alona IoT — Core

The main backend system of **Alona IoT**, running on a Raspberry Pi.

This repository contains the Elixir/Phoenix application responsible for:

- ingesting MQTT messages from ESP32 sensor nodes
- buffering and persisting measurements
- tracking device health and connectivity
- exposing APIs and real-time dashboards
- handling alerts and system health monitoring

The system is designed to run unattended for long periods, prioritizing resilience, fault isolation, and low operational maintenance.

## Responsibilities

- MQTT subscription and message validation
- Device registry and heartbeat tracking
- Buffered storage with backpressure handling
- Real-time UI via Phoenix LiveView
- System health and observability

## Non-Goals

- Cloud deployment
- Mobile applications
- Commercial multi-tenant features

## Related Repositories

- `firmware` — ESP32 sensor node firmware
- `protocol` — MQTT topics and payload schemas
- `infra` — deployment and operations
- `docs` — architecture and design documentation
