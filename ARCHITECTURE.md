# System Architecture

## High-Level Overview

VotePeace is designed as a **Decoupled Monolith**, where the frontend and backend reside in the same repository but operate as distinct, loosely coupled services.

## Architecture Diagram

```mermaid
graph TD
    User((User))
    Admin((Admin))
    
    subgraph Client [Frontend Layer]
        WebApp[React SPA \n(VotePeace-Frontend)]
    end
    
    subgraph Server [Backend Layer]
        API[Go Fiber API \n(VotePeace-Backend)]
        Auth[Auth Service \n(JWT/Bcrypt)]
        DB[(SQLite Database)]
    end
    
    User -->|HTTPS / JSON| WebApp
    Admin -->|HTTPS / JSON| WebApp
    
    WebApp -->|REST API Requests| API
    
    API -->|Auth Check| Auth
    API -->|Query/Transaction| DB
```

## Component Communication

### Frontend ↔ Backend
-   **Protocol**: HTTP/1.1 (REST)
-   **Data Format**: JSON
-   **Authentication**: JWT (JSON Web Tokens) or Session-based (depending on implementation).
-   **CORS**: The backend creates an allowlist for the frontend origin (`http://localhost:5173` in dev).

### Database Interaction
-   The Backend holds exclusive access to the SQLite database file.
-   No direct database access is allowed from the client.

## Design Patterns

-   **Backend**: MVC (Model-View-Controller) adapted for API use.
-   **Frontend**: Component-Based Architecture with Unidirectional Data Flow (Redux).

##Scalability Considerations

While currently functioning as a monolith with local storage (SQLite), the architecture allows for scaling:
1.  **Database**: GORM allows switching SQLite to PostgreSQL without code changes.
2.  **Containerization**: Both services can be individually containerized (Docker) and orchestrated (Kubernetes/Docker Compose).
