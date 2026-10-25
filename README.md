 <div align="center">

# :soccer: Fut Manager

</div>

This ecosystem implements a distributed microservices architecture designed for football management, tournament simulation, player tracking, and club administration.

---

## :book: Table of Contents

* [Overview](https://www.google.com/search?q=%23overview)
* [Microservices Ecosystem](https://www.google.com/search?q=%23microservices-ecosystem)
* [Tech Stack & Prerequisites](https://www.google.com/search?q=%23tech-stack--prerequisites)
* [Architecture Highlights](https://www.google.com/search?q=%23architecture-highlights)
* [Project Roadmap](https://www.google.com/search?q=%23project-roadmap)
* [Contributing](https://www.google.com/search?q=%23contributing)

---

## :mag: Overview

The **Fut Manager** platform is an open source project developed for software engineering coursework. It decouples core domain logic into dedicated, lightweight services orchestrated through a centralized Spring Cloud API Gateway and presented via a responsive user interface.

> [!NOTE]
> All backend domain microservices adhere to clean architectural principles, utilizing FastAPI for Python microservices, Java/Spring Boot for the API Gateway, and modern web frameworks for the client application.

---

## :triangular_ruler: Microservices Ecosystem

| Repository | Tech Stack | Primary Responsibility | Link |
| --- | --- | --- | --- |
| **Gateway** | Java / Spring Boot (Spring Cloud Gateway) | Central entry point, reactive request routing, filter management, and rate limiting | [View Repo](https://github.com/projetosoftware-2026-futebol/gateway) |
| **Frontend** | React / Next.js | Responsive user interface and match dashboards | [View Repo](https://github.com/projetosoftware-2026-futebol/frontend) |
| **Jogador (Player)** | Python / FastAPI | Player profile management, ratings, and market transactions | [View Repo](https://github.com/projetosoftware-2026-futebol/jogador) |
| **Clube (Club)** | Python / FastAPI | Club institutional data, budgets, stadiums, and squad rosters | [View Repo](https://github.com/projetosoftware-2026-futebol/clube) |
| **Jogos (Match)** | Python / FastAPI | Recording and scoring completed match fixtures | [View Repo](https://github.com/projetosoftware-2026-futebol/jogos) |

> [!WARNING]
> Ensure that environment variables and database connections are properly configured across all microservices before initiating local orchestration.

---

## :computer: Tech Stack & Prerequisites

Make sure your local environment meets the following requirements:

* Java JDK 17 or 21 (for Spring Boot API Gateway)
* Python 3.10+ (for backend FastAPI microservices)
* Node.js v18+ & package manager (for frontend)
* Docker & Docker Compose (for containerized multi-service deployment)

> [!TIP]
> Use Docker Compose to spin up the entire ecosystem simultaneously with pre-configured local networking.

---

## :gear: Architecture Highlights

* **Decoupled Domains:** Each service manages its own data store independently while exposing clean REST endpoints.
* **Standardized Communication:** RESTful APIs with JSON payloads and seamless bilingual support (Portuguese and English aliases).
* **Resilient Proxying:** The API Gateway abstracts internal network topologies and enforces security policies at the edge using Spring WebFlux reactive routing.
