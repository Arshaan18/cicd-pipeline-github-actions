# CI/CD Pipeline with GitHub Actions 🚀

## 📌 Project Overview
A fully automated CI/CD pipeline that builds, pushes, and deploys a Dockerized web application to AWS EC2 on every GitHub push — zero manual intervention required.

## ⚙️ How the Pipeline Works
1. Developer pushes code to GitHub (main branch)
2. GitHub Actions automatically triggers
3. Docker image is built from Dockerfile
4. Image is pushed to Docker Hub
5. GitHub Actions SSHs into AWS EC2
6. EC2 pulls the latest image and restarts the container
7. Updated webpage is live instantly

## 🛠 Tools & Technologies
- GitHub Actions (CI/CD automation)
- Docker & Dockerfile
- Nginx (Alpine base image)
- AWS EC2 (Ubuntu 24.04 LTS)
- Docker Hub (image registry)
- SSH (remote deployment)
- Linux & Bash

## 📁 Project Structure
cicd-pipeline/
├── index.html                    # Web app served by container
├── Dockerfile                    # Docker image blueprint
└── .github/
└── workflows/
└── deploy.yml            # GitHub Actions pipeline

## 🔐 GitHub Secrets Used
| Secret | Purpose |
|---|---|
| DOCKER_USERNAME | Docker Hub login |
| DOCKER_PASSWORD | Docker Hub password |
| EC2_HOST | AWS EC2 public IP |
| EC2_SSH_KEY | Private key for SSH access |

## 📸 Pipeline Result
![CI/CD Success](https://img.shields.io/badge/CI%2FCD-Passing-brightgreen)

## 👨‍💻 Author
**Arshaan Shaikh** — Fresher Cloud & DevOps Engineer
[LinkedIn](https://www.linkedin.com/in/arshaan-shaikh-95b61a227) | [GitHub](https://github.com/Arshaan18)
