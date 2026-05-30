# 🐳 Flask Container Lab

![Python](https://img.shields.io/badge/Python-3.x-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Flask](https://img.shields.io/badge/Flask-Web_App-000000?style=for-the-badge&logo=flask&logoColor=white)
![Podman](https://img.shields.io/badge/Podman-Containers-892CA0?style=for-the-badge&logo=podman&logoColor=white)
![nginx](https://img.shields.io/badge/nginx-Reverse_Proxy-009639?style=for-the-badge&logo=nginx&logoColor=white)
![Fedora](https://img.shields.io/badge/Fedora-Linux-294172?style=for-the-badge&logo=fedora&logoColor=white)
![DevOps](https://img.shields.io/badge/DevOps-Learning_Project-2496ED?style=for-the-badge)
![CI](https://img.shields.io/badge/CI-GitHub_Actions-2088FF?style=for-the-badge&logo=github-actions&logoColor=white)

---

## 📌 Overview

This project demonstrates the deployment of a **multi-container Flask application** using **Podman** and **nginx** on a Fedora Linux environment.

It focuses on containerized architecture, reverse proxy configuration, and internal container networking.

---

## ✨ Key Features

- 🐍 Flask backend application
- 📦 Containerized using Podman
- 🌐 nginx reverse proxy integration
- 🔗 Internal container networking
- ⚙️ Podman Compose orchestration
- 🖥️ Fedora Linux environment

---

## 🏗️ Architecture
```text
Client Browser
      ↓
nginx Reverse Proxy
      ↓
Flask Application Container
```
---

## 🚀 How to 

### 1. Clone the repository

```bash
git clone https://github.com/sgill3077/flask-container-lab.git
cd flask-container-lab
```
## 📂 Project Structure 

```text
flask-demo/
├── app/
│   ├── app.py
│   └── requirements.txt
├── nginx/
│   └── default.conf
├── compose.yaml
├── Containerfile
├── README.md
└── screenshots/
```
---

## ⚡ Project Status

Active Development

Planned improvements:

* Monitoring (Prometheus/Grafana integration)
* Centralized logging
* CI/CD pipeline automation
* Deployment hardening
---

## 🛠️ Tech Stack 

* Python 3
* Flask
* Podman
* Podman Compose
* nginx
* Fedora Linux
* GitHub Actions

---

## 🚀 Instructions 

### Build and Start Containers

```bash
podman compose up --build
```

### Open in Browser

```text
http://127.0.0.1:8080
```

### Stop Containers

```bash
podman compose down
```

---

## Current Functionality ✅

- Multi-container deployment
- Reverse proxy communication
- Internal container networking
- Containerized Flask application
- Declarative orchestration with Compose
- Local web application hosting

---

## 🔧 Future Work 

- Add persistent logging volumes
- Implement container health checks
- Integrate SSL/TLS support
- Add monitoring with Prometheus/Grafana
- Expand Flask application functionality
- Implement CI/CD workflows

---
## 📘 Purpose

This project was built for learning and portfolio demonstration, focusing on container orchestration and reverse proxy workflows in a Linux-based environment.

---
## GitHub Repository 🔗

Repository:
https://github.com/sgill3077/flask-container-lab
