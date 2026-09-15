# 🚀 MERN DevOps — GitHub Actions CI/CD

A **full-stack MERN application** demonstrating modern software development practices with **Docker containerization, GitHub Actions, CI/CD automation, and MongoDB**.

This project is designed to demonstrate how a MERN application can be developed, containerized, tested, and delivered using an automated DevOps workflow.

---

## 📌 Project Overview

This project combines a **React frontend**, **Node.js/Express backend**, and **MongoDB database** into a containerized full-stack application.

The project also demonstrates how **GitHub Actions** can automate the development lifecycle by running workflows whenever changes are pushed to the repository.

### 🎯 Key Objectives

* Build a full-stack MERN application
* Separate frontend and backend responsibilities
* Containerize application services using Docker
* Manage multiple services using Docker Compose
* Automate CI/CD using GitHub Actions
* Create a repeatable development environment
* Demonstrate modern DevOps practices

---

## 🏗️ Architecture

```text
                         ┌─────────────────────┐
                         │      Developer      │
                         │     Git / GitHub    │
                         └──────────┬──────────┘
                                    │
                                    │ Push / Pull Request
                                    ▼
                         ┌─────────────────────┐
                         │   GitHub Actions    │
                         │      CI / CD        │
                         └──────────┬──────────┘
                                    │
                          Build / Test / Package
                                    │
                                    ▼
                    ┌──────────────────────────────┐
                    │          Docker              │
                    │                              │
                    │  ┌────────┐   ┌──────────┐ │
                    │  │ React  │   │ Node.js  │ │
                    │  │ Client │──▶│ Express  │ │
                    │  └────────┘   └────┬─────┘ │
                    │                     │       │
                    │                     ▼       │
                    │                ┌─────────┐ │
                    │                │ MongoDB │ │
                    │                └─────────┘ │
                    └──────────────────────────────┘
```

---

## 🛠️ Tech Stack

### Frontend

* ⚛️ React
* JavaScript
* npm

### Backend

* 🟢 Node.js
* 🚂 Express.js
* REST APIs

### Database

* 🍃 MongoDB

### DevOps

* 🐳 Docker
* Docker Compose
* 🔄 GitHub Actions
* CI/CD Automation
* Git & GitHub

---

## ✨ Features

* Full-stack MERN architecture
* RESTful backend API
* React-based frontend
* MongoDB database integration
* Dockerized application environment
* Multi-container development with Docker Compose
* GitHub Actions workflow
* Automated CI/CD pipeline
* Reproducible development environment
* Separation of frontend and backend services

---

## 🔄 CI/CD Workflow

The project demonstrates a typical CI/CD lifecycle:

```text
Developer
    │
    ▼
Git Push
    │
    ▼
GitHub Repository
    │
    ▼
GitHub Actions
    │
    ├── Checkout Source
    │
    ├── Install Dependencies
    │
    ├── Build Application
    │
    ├── Run Validation / Tests
    │
    └── Build Docker Images
             │
             ▼
        Deploy / Release
```

This approach helps reduce manual deployment effort and provides a consistent software delivery process.

---

## 🐳 Docker

Docker is used to provide a consistent runtime environment across development and deployment.

### Docker Compose

The application services can be managed together using Docker Compose.

```bash
docker compose up --build
```

To run the services in the background:

```bash
docker compose up -d --build
```

To stop the application:

```bash
docker compose down
```

---

## 💻 Local Development

### 1. Clone the repository

```bash
git clone https://github.com/Kavinrajan/devops-mern-github-actions.git
```

```bash
cd devops-mern-github-actions
```

### 2. Install dependencies

Install the required dependencies for the frontend and backend according to their respective package configurations.

### 3. Configure environment variables

Create the required `.env` configuration for the backend and database connection.

Example:

```env
MONGO_URI=<your-mongodb-connection-string>
PORT=5000
```

> Do not commit secrets, credentials, API keys, or production environment variables to GitHub.

### 4. Start with Docker

```bash
docker compose up --build
```

---

## 📂 Project Structure

```text
devops-mern-github-actions/
│
├── .github/
│   └── workflows/
│       └── CI/CD workflow
│
├── frontend/
│   └── React application
│
├── backend/
│   └── Node.js / Express application
│
├── docker-compose.yml
│
├── Dockerfile
│
├── package.json
│
└── README.md
```

> The exact folder/file names may vary depending on the current implementation.

---

## 🔐 Environment Configuration

Environment-specific configuration should be kept outside the source code.

Typical configuration includes:

```text
MongoDB connection
Application port
Environment
Authentication / API secrets
Deployment configuration
```

Use GitHub Actions **Secrets and Variables** for sensitive CI/CD configuration.

---

## 📈 DevOps Practices Demonstrated

This project demonstrates several practices used in modern software engineering:

| Practice                    | Implementation           |
| --------------------------- | ------------------------ |
| Version Control             | Git / GitHub             |
| Frontend                    | React                    |
| Backend                     | Node.js + Express        |
| Database                    | MongoDB                  |
| Containerization            | Docker                   |
| Multi-container Environment | Docker Compose           |
| CI/CD                       | GitHub Actions           |
| Automation                  | GitHub Actions Workflows |
| Configuration               | Environment Variables    |
| Application Architecture    | MERN                     |

---

## 🎓 What I Learned

Through this project, I explored:

* Designing a MERN full-stack application
* Building REST APIs with Express
* Connecting Node.js applications with MongoDB
* Containerizing applications using Docker
* Managing multiple containers using Docker Compose
* Creating automated GitHub Actions workflows
* Understanding CI/CD pipelines
* Managing environment-specific configuration
* Applying DevOps practices to application development

---

## 🚀 Future Improvements

Possible enhancements include:

* [ ] Add automated unit and integration tests
* [ ] Add Docker image publishing
* [ ] Add deployment to a cloud platform
* [ ] Add production Docker configuration
* [ ] Add automated security scanning
* [ ] Add code-quality checks
* [ ] Add deployment notifications
* [ ] Add Kubernetes deployment
* [ ] Add monitoring and logging
* [ ] Add infrastructure-as-code

---

## 👨‍💻 About the Developer

**Kavinrajan S M**

Senior Android Developer | Kotlin | Android | Kotlin Multiplatform | AI/ML | Backend | DevOps

This project is part of my hands-on learning journey into **backend engineering, cloud-native development, AI/ML integration, and DevOps**, complementing my professional experience in Android application development.

### Core Areas

```text
Android Development
Kotlin
Jetpack Compose
Kotlin Multiplatform
Clean Architecture
REST APIs
Python
Machine Learning
FastAPI
Docker
CI/CD
GitHub Actions
```

---

## ⭐ Why This Project?

The goal of this project is to demonstrate that modern application development is not limited to writing application code.

A production-ready application also requires:

**Development → Testing → Containerization → Automation → CI/CD → Deployment**

This repository brings those concepts together in a practical MERN application.

---

## 📄 License

This project is intended for **learning and portfolio purposes**.

---

⭐ If you find this project useful, consider giving the repository a **star**.

