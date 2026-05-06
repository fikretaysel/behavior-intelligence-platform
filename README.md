````markdown
# Behavior Intelligence Platform (Symfony)

## Overview

A Symfony-based backend platform for scalable event tracking and behavior analytics infrastructure using event-driven architecture principles.

This project focuses on designing and implementing the core event tracking infrastructure required for collecting and processing user behavior data in modern analytics systems.

The long-term goal is to support:

- User journey analysis
- Conversion tracking
- Funnel analysis
- Drop-off detection
- Behavioral insights

---

## Purpose

Instead of directly building dashboards or analytics visualizations, this project focuses on the most important foundation:

**Capturing user behavior as structured events**

Modern e-commerce and analytics platforms start with scalable event collection architecture before building higher-level analytics features.

---

## Implemented Features

- Event entity architecture
- Flexible event structure with metadata support
- User and session tracking
- Scalable database model
- Symfony-based modular backend structure
- REST-oriented architecture foundation

---

## Architecture

The platform is designed using an event-driven architecture.

- User interactions are captured as immutable events
- Events are persisted for later analytics processing
- Asynchronous processing is planned using RabbitMQ
- Redis is used for caching and high-performance event workflows
- The architecture is designed for scalability and future distributed processing

---

## Tech Stack

- PHP 8
- Symfony
- Doctrine ORM
- MySQL
- Redis
- RabbitMQ
- Docker
- REST APIs

---

## Example Event

```json
{
  "eventType": "product_view",
  "userId": "123",
  "sessionId": "abc123",
  "page": "/product/45",
  "productId": "45",
  "metadata": {
    "price": 49.99
  }
}
```

---

## Planned Extensions

- Event ingestion API
- Funnel analysis
- User journey reconstruction
- Conversion tracking
- Real-time event processing
- Dashboard and visualization layer
- Distributed event processing architecture

---

## Run Locally

```bash
git clone https://github.com/fikretaysel/behavior-intelligence-platform.git

cd behavior-intelligence-platform

docker-compose up -d

composer install

php bin/console doctrine:migrations:migrate
```

---

## Why This Project Matters

Modern analytics platforms do not start with dashboards.

They start with scalable data collection infrastructure.

This project focuses on building that foundation correctly using modern backend engineering principles.

---

## Author

Fikret Aysel

---

## Status

🟡 In Progress — currently focused on backend event infrastructure and scalable event processing.
````
