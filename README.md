#  Behavior Intelligence Platform (Symfony)

##  Overview

This project is the **foundation of a Behavior Intelligence Platform** built with Symfony.

Currently, it focuses on designing and implementing the **event tracking infrastructure** that enables collecting user behavior data.

The long-term goal is to analyze:

* User journeys
* Conversion paths
* Funnel steps
* Drop-off points

---

##  Purpose

Instead of directly building a full analytics system, this project focuses on the **core building block**:

 Capturing user behavior as structured events

This is how modern e-commerce and analytics systems start.

---

##  Current Features

* Event entity design
* Flexible event structure (metadata support)
* User & session tracking
* Scalable data model for future analytics

---

##  Tech Stack

* PHP 8
* Symfony
* Doctrine ORM
* MySQL

---

##  Example Event

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

##  Architecture Idea

The system is designed around **event-based tracking**:

1. Every user action is stored as an event
2. Events can later be processed and analyzed
3. Higher-level insights (funnels, journeys) will be built on top of this

---

##  Planned Features

* Event ingestion API
* Funnel analysis
* User journey reconstruction
* Conversion tracking
* Real-time processing (RabbitMQ / Kafka)
* Dashboard & visualization

---

##  Why This Project Matters

Modern platforms don’t start with dashboards.

They start with **data collection architecture**.

This project focuses on building that foundation correctly.

---

##  Author

**Fikret Aysel**

---

##  Status

🟡 In Progress – currently focused on backend event infrastructure

---
