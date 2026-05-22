# Flask Container Lab

## Overview
This project demonstrates containerizing a Python Flask application using Podman on Fedora Linux. It focuses on reproducible container builds, container networking, and exposing a web service on a local network.

## Features
- Python Flask web application
- Podman Containerfile for building images
- Local network access testing
- Internal container networking

## Project Status
In Progress — expanding into multi-container architecture with nginx reverse proxy.

## Tech Stack
- Python
- Flask
- Podman
- Fedora Linux

## Instructions

1. Build the container image:
```bash
podman build -t flask-demo .

podman run -d -p 5000:5000 flask-demo

---

Add Future Work

```markdown

## Future Work
- Integrate with nginx reverse proxy using Podman Compose
- Add automated CI/CD deployment
- Include SSL/TLS with Let's Encrypt
- Expand API endpoint

## GitHub Links
[Project Repository](https://github.com/sgill3077/flask-container-lab)
