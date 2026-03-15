# 🚀 Automated CI/CD Pipeline for Dockerized Web App

This repository contains a full-stack CI/CD pipeline demonstrating automated deployment of a Python-based web application to AWS using Jenkins and Docker.

## 🏗️ Architecture
The pipeline follows a modern DevOps workflow to ensure code quality and rapid deployment:

1. **VCS:** Developer pushes code to **GitHub**.
2. **Build:** **Jenkins** triggers a build job via Webhooks.
3. **Containerize:** Jenkins builds a **Docker** image using a multi-stage `Dockerfile`.
4. **Test:** Automated unit tests are executed within the container environment.
5. **Deploy:** The image is pushed to a registry and deployed to an **AWS EC2** instance.
6. **Proxy:** **Nginx** acts as a reverse proxy to serve the application on Port 80.

## 🛠️ Tech Stack
* **CI/CD:** Jenkins (Declarative Pipeline)
* **Containers:** Docker & Docker Compose
* **Cloud:** AWS (EC2, Security Groups)
* **Web Server:** Nginx
* **Language:** Python (Flask) / Bash

## 📋 Key Features
- **Pipeline as Code:** Managed via a `Jenkinsfile`.
- **Environment Isolation:** Using Docker to ensure "it works on my machine" translates to production.
- **Zero-Downtime Strategy:** Simple container restart logic with Nginx health checks.

## 🚦 Getting Started
1. Ensure Jenkins is installed with the Docker pipeline plugin.
2. Add your AWS SSH keys to Jenkins credentials.
3. Run the pipeline by pointing Jenkins to this repo's `main` branch.
