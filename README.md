# Kafka Monitoring with Prometheus & Grafana

## Objective
Building a Proof of Concept (PoC) to monitor Consumer Lag in a high-throughput event ingestion pipeline.

## Architecture
- **Producer:** Python script simulating Cloud Log Ingestion (AWS/Azure logs).
- **Broker:** Apache Kafka.
- **Exporter:** Kafka Exporter (to expose metrics).
- **Visualization:** Grafana Dashboard tracking `kafka_consumergroup_lag`.

## Why?
In event-driven security architecture, "Real-time" detection fails if consumer lag spikes. This project solves observability for that bottleneck.
