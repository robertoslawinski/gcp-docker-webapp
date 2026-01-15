

# 🚀 Cloud Deployment Project — CI/CD on Google Cloud

This project demonstrates a complete cloud deployment pipeline using modern DevOps and Cloud Engineering practices.

A web application is deployed on a Google Cloud VM using Docker and is automatically updated through a CI/CD pipeline powered by GitHub Actions.

Live Demo:
**[http://35.240.91.141](http://35.240.91.141)**

---

## 🧱 Architecture Overview

```
Developer → GitHub → GitHub Actions → SSH → Google Cloud VM → Docker → Nginx → Web App
```

---

## 🛠️ Technologies Used

| Area           | Stack                     |
| -------------- | ------------------------- |
| Cloud Provider | Google Cloud Platform     |
| Compute        | Compute Engine VM (Linux) |
| Containers     | Docker                    |
| Web Server     | Nginx                     |
| CI/CD          | GitHub Actions            |
| Security       | SSH, Firewall Rules       |
| Automation     | GitHub Workflows          |

---

## ⚙️ How It Works

1. Code is pushed to the `main` branch on GitHub.
2. GitHub Actions triggers a deployment workflow.
3. The pipeline connects securely to the VM via SSH.
4. The application is rebuilt as a Docker image.
5. The running container is replaced with the new version.
6. The updated website is instantly available.

This ensures **zero-downtime updates** and full automation.

---

## 🧪 CI/CD Workflow

The deployment process is fully automated using this workflow:

```
.github/workflows/deploy.yml
```

It performs:

* Git clone / pull
* Docker image build
* Container replacement
* Service validation

---

## 🧩 Project Structure

```
.
├── Dockerfile
├── index.html
├── README.md
└── .github
    └── workflows
        └── deploy.yml
```

---

## 🔐 Security & Reliability

* SSH authentication with private keys
* Firewall rules exposing only required ports
* Immutable Docker deployments
* Automated recovery on redeploy

---

## 👨‍💻 Author

**Roberto Slawinski**
Cloud & DevOps Engineering Student
Portugal · 2026

---

