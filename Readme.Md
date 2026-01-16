# VotePeace - Modern Electronic Voting Platform

![VotePeace Status](https://img.shields.io/badge/status-active-success.svg)
![License](https://img.shields.io/badge/license-MIT-blue.svg)

**VotePeace** is an enterprise-grade, secure, and transparent electronic voting platform designed to streamline elections for organizations of all sizes. It ensures integrity, real-time analytics, and a seamless user experience for both voters and administrators.

## 🌟 Project Overview

VotePeace solves the challenge of manual, error-prone voting processes by providing a digital-first solution. It features a robust backend for secure vote processing and a modern, responsive frontend for an engaging voter experience.

### Key Capabilities
-   **Security First**: Encrypted vote storage and secure authentication.
-   **Real-Time Analytics**: Instant visualization of election results.
-   **Cross-Platform**: Optimized for web and mobile devices.
-   **Scalable Architecture**: Modular design separating concern between client and server.

## 📂 Repository Structure Overview

This repository uses a **Monorepo** structure to house both the server-side and client-side applications.

```
VotePeace/
├── VotePeace-Backend/   # Go (Fiber) + SQLite API Server
├── VotePeace-Frontend/  # React (Vite) + MUI Client Application
├── ARCHITECTURE.md      # System-wide Architecture Documentation
└── README.md            # You are here
```

## 🏗 Sub-Projects Description

| Project | Tech Stack | Description | README |
| :--- | :--- | :--- | :--- |
| **Backend** | Go, Fiber, GORM, SQLite | The core API server handling auth, business logic, and database persistence. | [Read Docs](./VotePeace-Backend/README.md) |
| **Frontend** | React 19, Vite, MUI v7 | The responsive web interface for voters and admins. | [Read Docs](./VotePeace-Frontend/README.md) |

## 🚀 Getting Started

To get the entire system running locally:

### Prerequisites
-   Go 1.21+
-   Node.js 20+
-   Git

### Quick Start
1.  **Clone the Repository**:
    ```bash
    git clone https://github.com/MDF05/VotePeace.git
    cd VotePeace
    ```

2.  **Setup Backend**:
    ```bash
    cd VotePeace-Backend
    go mod tidy
    go run main.go
    ```
    *Server runs at `http://localhost:3000`*

3.  **Setup Frontend** (New Terminal):
    ```bash
    cd VotePeace-Frontend
    npm install
    npm run dev
    ```
    *Client runs at `http://localhost:5173`*

## 📚 Documentation

Detailed documentation for the entire platform:

| Document | Description |
| :--- | :--- |
| [**System Architecture**](./ARCHITECTURE.md) | High-level system design and communication flow. |
| [**Governance**](./GOVERNANCE.md) | Decision-making process and project roles. |
| [**Contribution Guide**](./CONTRIBUTING.md) | Guidelines for specialized contribution workflows. |
| [**Code of Conduct**](./CODE_OF_CONDUCT.md) | Community standards and enforcement. |
| [**Security Policy**](./SECURITY.md) | Vulnerability reporting and security protocols. |
| [**Changelog**](./CHANGELOG.md) | Global release history and version tracking. |
| [**Roadmap**](./ROADMAP.md) | Future milestones and strategic goals. |
| [**Support**](./SUPPORT.md) | Resources for getting help. |
| [**Disclaimer**](./DISCLAIMER.md) | Legal limitations and usage warnings. |
| [**License**](./LICENSE) | MIT License details. |

## 🤝 Contribution Flow

We follow a strict **Fork & Pull Request** workflow.
1.  Fork the repo.
2.  Create a feature branch.
3.  Commit changes (Conventional Commits).
4.  Open a Pull Request against `main`.

See [CONTRIBUTING.md](./CONTRIBUTING.md) for details.

## 🔐 Security

Security is paramount. Please adhere to the policies outlined in [SECURITY.md](./SECURITY.md). Do not report vulnerabilities on public issues.

## 📄 License

This project is licensed under the MIT License. See [LICENSE](./LICENSE).

## 👤 Maintainers

**Muhammad Dava Fahreza**
-   GitHub: [@MDF05](https://github.com/MDF05)