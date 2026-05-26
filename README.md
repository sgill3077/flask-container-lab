# Flask Container Lab 🐳

## Overview 📝

This project demonstrates deploying a multi-container Flask application environment using Podman and nginx on Fedora Linux. The lab focuses on container orchestration, reverse proxy configuration, internal container networking, and reproducible application deployment workflows.

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
Project Structure 📂
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
Project Status ⚡

Active Development — core multi-container architecture completed and expanding with monitoring, logging, and deployment enhancements.

Tech Stack 🛠️
Python 3
Flask
Podman
Podman Compose
nginx
Fedora Linux
Instructions 🚀
1. Build and Start Containers
podman compose up --build
2. Open in Browser
http://127.0.0.1:8080
3. Stop Containers
podman compose down
Current Functionality ✅
Multi-container deployment
Reverse proxy communication
Internal container networking
Containerized Flask application
Declarative orchestration with Compose
Local web application hosting
Future Work 🔧
Add persistent logging volumes
Implement container health checks
Integrate SSL/TLS support
Add monitoring with Prometheus/Grafana
Expand Flask application functionality
Implement CI/CD workflows
GitHub Repository 🔗

GitHub: https://github.com/sgill3077/flask-container-lab
