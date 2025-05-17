# 🛡️ SentinelFlux

**SentinelFlux** is a secure, real-time incident response platform tailored for Security Operations Centers (SOCs) and threat monitoring teams. Built with **React.js**, **Spring Boot**, **WebSockets**, and **Kafka**, it facilitates fast, role-based decision-making and team coordination during live security events.

The platform uses a **microservice architecture** with containerized services for incident tracking, real-time alert feeds, analyst messaging, and audit logging. It is fully Dockerized and scalable via Kubernetes or Podman.

## 📌 Features

- ⚠️ **Incident Feed Dashboard**:
  - Live incident push updates via WebSockets
  - Categorized alerts (malware, insider threat, physical breach)
  - Status tracking: new, in progress, resolved

- 👥 **Role-Based Access**:
  - Separate UIs and access levels for analysts, leads, admins
  - JWT authentication with secure session tokens

- 💬 **Team Collaboration**:
  - Analyst-to-analyst secure messaging via WebSockets
  - Context-linked discussions for each incident

- 📊 **Analytics & Audit Logs**:
  - Historical incident data stored in PostgreSQL
  - MongoDB for audit trails and activity logs
  - Charts showing response time, frequency by category

- 🚀 **Containerized & Scalable**:
  - Microservices deployed via Docker and Kubernetes
  - Kafka for event streaming between alert sources and services

## 🛠️ Tech Stack

- **Frontend**: React.js, WebSockets, Chart.js
- **Backend**: Java, Spring Boot, Kafka
- **Databases**: PostgreSQL, MongoDB
- **Containers**: Docker, Kubernetes or Podman
- **Security**: OAuth2, JWT, HTTPS

## 🚀 Getting Started

### Prerequisites

- Java 17+
- Node.js 18+
- Docker & Docker Compose
- PostgreSQL & MongoDB instances

### Clone & Deploy

```bash
git clone https://github.com/your-username/sentinelflux.git
cd sentinelflux
docker-compose up --build
