# Flask Container Lab 🐳

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
