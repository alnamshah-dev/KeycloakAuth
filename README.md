# KeycloakAuth
This repository contains a complete, containerized application stack demonstrating a modern microservices architecture. It includes a secure .NET Web API, an API Gateway, a Keycloak identity server, and Jaeger for distributed tracing.

The entire system is orchestrated with `docker-compose`, allowing you to launch all services with a single command.

## Architecture Overview

This project consists of four main services working together:

1.  **`keycloak.auth.proxy` (API Gateway)**
2.  **`keycloak.auth.api` (.NET Backend Service)**: The core business logic resides here. This service is protected by Keycloak and handles the main functionality of the application.
3.  **`keycloak` (Identity Server)**: The centralized authentication and authorization service. It manages users, roles, and issues JWTs.
4.  **`jaeger` (Distributed Tracing)**: Collects and visualizes traces from both the API Gateway and the backend service, providing end-to-end observability of requests.

## Key Features

-   **Docker-Compose Setup**: Launch the entire multi-service stack with one command.
-   **Secure Authentication**: The backend API (`keycloak.auth.api`) is secured using JWTs from Keycloak.
-   **End-to-End Observability**: Distributed tracing is enabled across the gateway and the API using **Jaeger** and **OpenTelemetry**.
-   **Persistent Data**: Keycloak data is persisted in a Docker volume, so users and configurations are not lost on restart.

##  🛠️ Tech Stack

⚙️ **Backend** | [.NET 8](https://dotnet.microsoft.com/), [ASP.NET Core](https://learn.microsoft.com/aspnet/core) |
| 🧩 **Containerization** | [Docker](https://www.docker.com/) & [Docker Compose](https://docs.docker.com/compose/) |
| 🔐 **Identity & Access** | [Keycloak](https://www.keycloak.org/) |
| 📡 **Observability** | [Jaeger](https://www.jaegertracing.io/) + [OpenTelemetry](https://opentelemetry.io/) |


### 🧾 Tech Badges

![.NET](https://img.shields.io/badge/.NET%208.0-512BD4?logo=dotnet&logoColor=white)
![ASP.NET Core](https://img.shields.io/badge/ASP.NET%20Core-5C2D91?logo=dotnet&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?logo=docker&logoColor=white)
![Keycloak](https://img.shields.io/badge/Keycloak-000000?logo=keycloak&logoColor=white)
![Jaeger](https://img.shields.io/badge/Jaeger-FF6C37?logo=jaeger&logoColor=white)
![OpenTelemetry](https://img.shields.io/badge/OpenTelemetry-6E45B7?logo=opentelemetry&logoColor=white)
