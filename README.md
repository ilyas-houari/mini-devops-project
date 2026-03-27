# DevOps Mini Project

## 📌 Description
This project implements a CI/CD pipeline for a multi-container application using DevOps tools.

## 🧱 Architecture
- Node.js backend (Express)
- MongoDB database
- Docker & Docker Compose

## ⚙️ Tools Used
- GitHub → Source code management
- GitHub Actions → Continuous Integration
- Jenkins → CI/CD pipeline orchestration
- Docker → Containerization
- Docker Compose → Multi-container orchestration
- SonarQube → Code quality (concept)
- Slack → Notifications (concept)
- Webhook → GitHub triggers Jenkins

## 🔄 CI/CD Pipeline
1. Developer pushes code to GitHub
2. GitHub Actions runs tests
3. Webhook triggers Jenkins
4. Jenkins builds Docker image
5. Application is deployed with Docker Compose

## ▶️ How to Run
```bash
docker build -t devops-app .
docker-compose up