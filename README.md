# Microservices Architecture: Serverless vs Serverful Performance

This project compares the performance of serverless and serverful deployments using a Django-based microservices architecture. The system includes three services: **polls**, **questions**, and **votes**.

## Highlights

- Built and containerized each microservice using Docker.
- Deployed serverful setup with Docker Compose.
- Deployed serverless version using Google Cloud Endpoints.
- Monitored latency and response time with Grafana.
- Compared performance between both deployment models.

## Results

| Metric        | Serverful | Serverless |
|---------------|-----------|------------|
| Latency       | 72 ms     | 49 ms      |
| Response Time | 153 ms    | 90 ms      |

## Tech Stack

- Django
- PostgreSQL
- Docker & Docker Compose
- Google Cloud Platform (GCP)
- Grafana

## Folder Overview

Each microservice (polls, questions, votes) is in its own folder under `django-microservices/`. The setup includes:

- `docker-compose.yml` for local/serverful deployment
- `api_gateway.yml` for GCP serverless deployment

## Summary

This repository demonstrates how architectural choices impact application performance. It serves as a benchmark for evaluating microservices under different deployment strategies.
