# 🐳 Flask Container Lab

![Python](https://img.shields.io/badge/Python-3.x-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Flask](https://img.shields.io/badge/Flask-Web_App-000000?style=for-the-badge&logo=flask&logoColor=white)
![Podman](https://img.shields.io/badge/Podman-Containers-892CA0?style=for-the-badge&logo=podman&logoColor=white)
![nginx](https://img.shields.io/badge/nginx-Reverse_Proxy-009639?style=for-the-badge&logo=nginx&logoColor=white)
![Fedora](https://img.shields.io/badge/Fedora-Linux-294172?style=for-the-badge&logo=fedora&logoColor=white)
![CI](https://github.com/sgill3077/flask-container-lab/actions/workflows/python-ci.yml/badge.svg)
---

## 📌 Overview

This project demonstrates the deployment of a multi-container Flask application using Podman and nginx on Fedora Linux.

The lab focuses on:

- Containerized application deployment
- Reverse proxy configuration
- Internal container networking
- Podman Compose orchestration

---

## ✨ Current Functionality

- Multi-container deployment
- Reverse proxy communication
- Internal container networking
- Containerized Flask application
- Declarative orchestration with Compose
- Local web application hosting

---

## 🏗️ Architecture

```text
Browser
   │
localhost:8080
   │
   ▼
nginx Container
   │
   ▼
Flask Container
```

---

## 📸 Deployment Verification

### Running Containers

![Running Containers](screenshots/podman-ps.png)

### Application Response

![Application Response](screenshots/application-page.png)

### Curl Test

![Curl Test](screenshots/curl-test.png)

---

## 📂 Project Structure

```text
flask-demo/
├── app/
│   ├── app.py
│   └── requirements.txt
├── nginx/
│   └── default.conf
├── screenshots/
├── Containerfile
├── compose.yaml
└── README.md
```

---

## 🚀 Getting Started

### Clone the Repository

```bash
git clone https://github.com/sgill3077/flask-container-lab.git
cd flask-container-lab
```

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

## 🛠️ Tech Stack

- Python 3
- Flask
- Podman
- Podman Compose
- nginx
- Fedora Linux

---

## 📘 Purpose

This project was built for learning and portfolio demonstration, focusing on containerization, reverse proxy workflows, and container networking in a Linux environment.

---

## 🔧 Future Work

- Add persistent logging volumes
- Implement container health checks
- Integrate SSL/TLS support
- Add monitoring with Prometheus/Grafana
- Implement CI/CD workflows

---

## GitHub Repository 🔗

Repository:

https://github.com/sgill3077/flask-container-lab
