# KeycloakAuth
# .NET API with Keycloak Authentication

This repository showcases a secure .NET Web API integrated with **Keycloak** for robust authentication and authorization. The project demonstrates how to protect API endpoints using JSON Web Tokens (JWTs) issued by an external identity provider, following modern security best practices.

This project is designed to be a clean, practical reference for developers looking to implement token-based security in their .NET applications.

## Key Features

-   **Secure Authentication**: Implements JWT Bearer token authentication to protect API endpoints.
-   **Keycloak Integration**: Configured to use Keycloak as the OpenID Connect (OIDC) identity provider for centralized user management.
-   **Role-Based Authorization**: Includes examples of how to restrict access to certain endpoints based on user roles defined in Keycloak.
-   **Swagger/OpenAPI Support**: The Swagger UI is fully configured to handle the OAuth2 authentication flow, allowing for easy testing of protected endpoints directly from the browser.
-   **Configuration-Driven**: All Keycloak-related settings are managed in `appsettings.json`, allowing for easy environment-specific configuration.

## Tech Stack

-   **.NET 8** (or your version) - A fast, modern, and cross-platform framework for building web APIs.
-   **Keycloak** - An open-source Identity and Access Management (IAM) solution.
-   **Docker** - Used for running a local instance of Keycloak.
