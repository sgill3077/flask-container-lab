# 🐳 Flask Container Lab

![Python](https://img.shields.io/badge/Python-3.x-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Flask](https://img.shields.io/badge/Flask-Web_App-000000?style=for-the-badge&logo=flask&logoColor=white)
![Podman](https://img.shields.io/badge/Podman-Containers-892CA0?style=for-the-badge&logo=podman&logoColor=white)
![nginx](https://img.shields.io/badge/nginx-Reverse_Proxy-009639?style=for-the-badge&logo=nginx&logoColor=white)
![Fedora](https://img.shields.io/badge/Fedora-Linux-294172?style=for-the-badge&logo=fedora&logoColor=white)
![Container Networking](https://img.shields.io/badge/Container-Networking-success?style=for-the-badge)
![Infrastructure Lab](https://img.shields.io/badge/Infrastructure-Lab-orange?style=for-the-badge)
![DevOps](https://img.shields.io/badge/DevOps-Learning_Project-2496ED?style=for-the-badge)

## Overview 📝

This project demonstrates deploying a multi-container Flask application environment using Podman and nginx on Fedora Linux.

The lab focuses on:
- container orchestration
- reverse proxy configuration
- internal container networking
- reproducible deployment workflows

---

## Features ✨

- 🐍 Python Flask web application
- 📦 Podman containerized deployment
- 🌐 nginx reverse proxy integration
- 🔗 Internal container networking
- ⚙️ Podman Compose orchestration
- 🖥️ Fedora Linux host environment

---

## Architecture 🏗️

```text
Client Browser
      ↓
nginx Reverse Proxy
      ↓
Flask Application Container
```

---

## Project Structure 📂

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

## Project Status ⚡

Active Development — core multi-container architecture completed and expanding with monitoring, logging, and deployment enhancements.

---

## Tech Stack 🛠️

- Python 3
- Flask
- Podman
- Podman Compose
- nginx
- Fedora Linux

---

## Instructions 🚀

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

## Future Work 🔧

- Add persistent logging volumes
- Implement container health checks
- Integrate SSL/TLS support
- Add monitoring with Prometheus/Grafana
- Expand Flask application functionality
- Implement CI/CD workflows

---

## GitHub Repository 🔗

Repository:
https://github.com/sgill3077/flask-container-lab
