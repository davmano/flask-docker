# 🚀 Docker Simple Web App

This project demonstrates how to containerize a basic Python Flask application using Docker.

---

## ✅ Features
- Python Flask minimal web server
- Dockerfile-based containerization
- Port mapping from container to host
- Lightweight and fast

---

## 📂 Project Structure

```bash
docker-simple-webapp/
├── app.py
├── Dockerfile
└── README.md
```

#  Docker Flask App Deployment with GitHub Actions

[![Docker Build and Push](https://github.com/davmano/flask-docker/actions/workflows/docker-publish.yml/badge.svg)](https://github.com/davmano/flask-docker/actions)

---

## 🖼 Architecture Diagram
```
+----------------------------------+
|        Local Development         |
|    (VSCode / Pycharm + Git)       |
+----------------------------------+
               |
               | (git push)
               ↓
+----------------------------------+
|            GitHub                |
| Repo: docker-simple-webapp       |
| Action: docker-publish.yml       |
+----------------------------------+
               |
               | (GitHub Actions CI/CD)
               ↓
+----------------------------------+
|         GitHub Actions           |
| - Build Docker Image             |
| - Login to Docker Hub (using Secrets) |
| - Push Docker Image to Docker Hub |
+----------------------------------+
               |
               | (New Image Available)
               ↓
+----------------------------------+
|         Docker Hub               |
| Repo: davmano/docker-simple-webapp |
+----------------------------------+
               |
               | (Pull for Deployments later)
               ↓
+----------------------------------+
|  Future: AWS ECS, Kubernetes, etc. |
+----------------------------------+
```

