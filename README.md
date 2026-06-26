# 🚀 Nexa AI – Intelligent Sales Agent Platform

<p align="center">
  <img src="docs/logo.png" width="180" alt="Nexa AI Logo">
</p>

<p align="center">
  <strong>An AI-powered, self-hostable Sales Agent Platform that enables businesses to deploy intelligent shopping assistants with automated product recommendations, inventory awareness, Telegram integration, and one-click cloud deployments.</strong>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Node.js-18+-green">
  <img src="https://img.shields.io/badge/Docker-Containerized-blue">
  <img src="https://img.shields.io/badge/gRPC-Microservices-orange">
  <img src="https://img.shields.io/badge/Traefik-Reverse%20Proxy-purple">
  <img src="https://img.shields.io/badge/License-MIT-success">
</p>

---

# 📖 Overview

Nexa AI is a production-ready AI Sales Agent platform that enables businesses to launch intelligent shopping assistants in minutes.

The platform automatically deploys customer AI agents inside isolated Docker containers, provisions secure HTTPS domains using Traefik, and allows customers to interact through Telegram or the web.

Instead of building individual chatbots for every business, Nexa AI acts as a Platform-as-a-Service (PaaS), where each customer receives their own AI-powered shopping assistant running in an isolated environment.

---

# ✨ Features

## 🤖 AI Sales Assistant

- Natural language conversations
- Personalized product recommendations
- Product search
- Product comparison
- Inventory-aware recommendations
- Frequently Asked Questions
- Context-aware conversations

---

## 🛍 Product Recommendation Engine

- Intelligent product search
- Inventory availability checks
- Gender & category filtering
- Quantity validation
- Pagination support
- Product ranking

---

## 🏪 Inventory Management

- Real-time inventory lookup
- Store inventory
- Warehouse inventory
- Availability validation
- Stock quantity calculation

---

## 📱 Telegram Integration

- Telegram Bot support
- Secure Webhooks
- AI Conversations
- Instant customer support
- Rich message responses

---

## 🌐 Deployment Platform

Every customer project is automatically deployed as an isolated application.

Features include:

- Docker container creation
- Automatic image deployment
- Reverse proxy configuration
- HTTPS provisioning
- Custom subdomains
- Health monitoring
- Automatic restarts

---

## ⚡ Microservice Architecture

The platform follows a distributed microservice architecture.

```
                    User
                      │
          Telegram / Web Client
                      │
                      ▼
            Orchestrator Service
                      │
      ┌───────────────┼────────────────┐
      │               │                │
      ▼               ▼                ▼
Conversation     Recommendation     Inventory
    Agent             Agent            Agent
      │
      ▼
 Product Catalog & Business Logic
```

Each AI capability is isolated into its own gRPC service, making the platform modular, scalable, and easy to maintain.

---

# 🏗 System Architecture

```
                GitHub Repository
                       │
               GitHub Actions
                       │
                       ▼
              Docker Image Build
                       │
                       ▼
            GitHub Container Registry
                       │
                       ▼
            Nexa Deployment Service
                       │
          Creates Customer Container
                       │
          Connects to Traefik Network
                       │
                       ▼
              HTTPS Customer URL
```

---

# 🛠 Technology Stack

## Backend

- Node.js
- Express.js
- gRPC
- Docker
- Traefik

## AI

- Large Language Models
- Prompt Engineering
- Retrieval-based Recommendations
- Intent Routing

## DevOps

- Docker
- Docker Hub / GitHub Container Registry
- GitHub Actions
- Reverse Proxy
- HTTPS Automation

## Integrations

- Telegram Bot API
- GitHub API
- Container Registry

---

# 📂 Project Structure

```
.
├── agents/
│   ├── conversationAgent.js
│   ├── recommendationAgent.js
│   ├── inventoryAgent.js
│   └── ...
│
├── orchestrator/
│   ├── index.js
│   ├── routes.js
│   └── ...
│
├── proto/
│   └── agents.proto
│
├── data/
│   ├── inventory.json
│   └── productCatalog.json
│
├── docs/
├── Dockerfile
├── docker-compose.yml
└── README.md
```

---

# ⚙️ Deployment Workflow

```
Create Project
      │
      ▼
Connect GitHub Repository
      │
      ▼
Generate Deployment Config
      │
      ▼
GitHub Actions Builds Docker Image
      │
      ▼
Push Image to Registry
      │
      ▼
Deployment Service
      │
      ▼
Launch Docker Container
      │
      ▼
Traefik Routing
      │
      ▼
HTTPS Live Application
```

---

# 🔒 Security

- HTTPS by default
- Docker container isolation
- Secure deployment keys
- GitHub App authentication
- Environment-based configuration
- Inventory validation
- Request validation

---

# 🚀 Scalability

Designed for horizontal scaling.

- Independent microservices
- Stateless services
- Containerized deployments
- Reverse proxy routing
- Easy service expansion
- Supports multiple customer deployments

---

# 💡 Use Cases

- AI Shopping Assistant
- E-commerce Customer Support
- Retail Automation
- Product Recommendation Platform
- AI Sales Representative
- Customer Engagement Bot

---

# 📈 Future Improvements

- Voice AI Support
- WhatsApp Integration
- Admin Dashboard
- Customer Analytics
- Order Placement
- Payment Integration
- CRM Integration
- RAG Knowledge Base
- Multi-language Support

---

# 👨‍💻 Author

**Jeganath B**

Full Stack Developer | AI Enthusiast | Cloud & DevOps

- GitHub: https://github.com/jeganath18
- LinkedIn: https://linkedin.com/in/jeganath18

---

# ⭐ Why This Project?

Nexa AI demonstrates the design and implementation of a production-grade AI platform by combining microservices, container orchestration, AI-powered recommendation systems, cloud deployment automation, and conversational interfaces into a scalable Platform-as-a-Service (PaaS). The project highlights expertise in distributed systems, backend engineering, DevOps, API integrations, and applied AI for real-world business solutions.
