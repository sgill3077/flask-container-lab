# 🐳 Flask Container Lab

![Python](https://img.shields.io/badge/Python-3.x-3776AB?style=for-the-badge\&logo=python\&logoColor=white)
![Flask](https://img.shields.io/badge/Flask-Web_App-000000?style=for-the-badge\&logo=flask\&logoColor=white)
![Podman](https://img.shields.io/badge/Podman-Containers-892CA0?style=for-the-badge\&logo=podman\&logoColor=white)
![nginx](https://img.shields.io/badge/nginx-Reverse_Proxy-009639?style=for-the-badge\&logo=nginx\&logoColor=white)
![Fedora](https://img.shields.io/badge/Fedora-Linux-294172?style=for-the-badge\&logo=fedora\&logoColor=white)
![CI](https://github.com/sgill3077/flask-container-lab/actions/workflows/python-ci.yml/badge.svg)

---

# 📌 Overview
This project demonstrates the deployment of a multi-container Flask application using Podman and nginx on Fedora Linux.

The environment now includes Prometheus-compatible application metrics, enabling observability and future monitoring integration with Prometheus and Grafana.

The lab focuses on:

- Containerized application deployment
- Reverse proxy configuration
- Internal container networking
- Application instrumentation
- Metrics exposure for observability
- Podman Compose orchestration

---

# ✨ Current Functionality

* Multi-container deployment
* Reverse proxy communication
* Internal container networking
* Containerized Flask application
* Prometheus-compatible metrics exposure
* HTTP request monitoring
* Declarative orchestration with Compose
* Local web application hosting

---

# 🧠 Key Concepts Demonstrated

* Linux container workflows
* Reverse proxy configuration
* Container networking
* Multi-container orchestration
* Service isolation
* Declarative infrastructure configuration
* CI/CD fundamentals
* Web application deployment

---

# 🏗️ Architecture

Client Browser
      │
      ▼
nginx Reverse Proxy Container
      │
      ▼
Flask Application Container
      │
      ├── Application Responses
      │
      └── /metrics Endpoint
               │
               ▼
     Prometheus-Compatible Metrics

Internal Podman Network
```

## Traffic Flow

1. Client requests arrive through nginx on port 8080
2. nginx forwards requests to the Flask application container
3. Flask processes application requests and returns responses
4. Flask exposes Prometheus-compatible metrics through `/metrics`
5. Containers communicate through an isolated internal Podman network
---

# ⚙️ Continuous Integration

This project includes a GitHub Actions CI workflow that automatically:

* Validates Python dependencies
* Installs application requirements
* Runs verification checks
* Validates repository changes on push and pull requests

The CI pipeline helps ensure deployment consistency and improves development workflow reliability.

---

# 📸 Deployment Verification

## Running Containers

![Running Containers](screenshots/podman-ps.png)

## Application Response

![Application Response](screenshots/application-page.png)

## Curl Test

![Curl Test](screenshots/curl-test.png)

---

# 📂 Project Structure

```text
flask-container-lab/
├── app/
│   ├── app.py
│   └── requirements.txt
├── nginx/
│   └── default.conf
├── screenshots/
├── .github/workflows/
├── Containerfile
├── compose.yaml
└── README.md
```

---

# 🚀 Getting Started

## Clone the Repository

```bash
git clone https://github.com/sgill3077/flask-container-lab.git
cd flask-container-lab
```

## Build and Start Containers

```bash
podman compose up --build
```

## Open in Browser

```text
http://127.0.0.1:8080
```

## Stop Containers

```bash
podman compose down
```

---

# 🛠️ Tech Stack

* Python 3
* Flask
* Podman
* Podman Compose
* nginx
* GitHub Actions
* Fedora Linux

---

# 📚 Lessons Learned

Through this project I gained practical experience with:

* Configuring nginx as a reverse proxy
* Debugging container networking issues
* Managing multi-container environments
* Building reproducible deployment workflows
* Working with Podman Compose on Linux systems
* Implementing basic CI automation workflows

The project also improved my understanding of service communication and infrastructure troubleshooting in containerized environments.

---

# 📈 Prometheus Metrics Integration

The Flask application now exposes Prometheus-compatible metrics through:

```text
/metrics
```

Example endpoint:

```text
http://127.0.0.1:8080/metrics
```

Current metrics include:

* HTTP request counters
* Python runtime metrics
* Process-level metrics

This instrumentation enables future integration with Prometheus and Grafana for observability and monitoring workflows.


---

# 🔧 Future Improvements

* Add persistent logging volumes
* Implement container health checks
* Integrate SSL/TLS support
* Integrate Prometheus scraping and Grafana dashboards
* Expand CI/CD automation workflows
* Deploy to a cloud-hosted Linux VM

---

# 🔗 GitHub Repository

Repository:

https://github.com/sgill3077/flask-container-lab
