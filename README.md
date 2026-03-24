
# DevOps CI/CD Pipeline Project

##  Project Overview

This project demonstrates an **end-to-end CI/CD pipeline** using GitHub Actions, Docker, and AWS EC2.

Whenever code is pushed to the repository, the pipeline automatically:

* Builds the application
* Creates a Docker image
* Deploys the application to a server

---

##  Workflow (How It Works)

### 1️⃣ Code Push

Developer pushes code to GitHub repository.

### 2️⃣ CI Pipeline Triggered

GitHub Actions automatically starts the pipeline.

### 3️⃣ Build Process

* Code is checked out
* Docker image is built

### 4️⃣ Deployment (CD)

* Application is deployed to server (EC2)
* Old container is replaced with new one

### 5️⃣ Application Live

App becomes available via public IP.


## 🛠️ Tech Stack

* GitHub Actions (CI/CD)
* Docker
* AWS EC2
* Python (Flask)

---

## 📂 Project Structure

```
devops-cicd-project/
│
├── app/
├── Dockerfile
├── docker-compose.yml
├── .github/workflows/
└── README.md
```

---

## 🚀 How to Run Locally

```bash
docker build -t devops-app .
docker run -d -p 80:5000 devops-app
```


## 🎯 Key Features

* Automated CI/CD pipeline
* Containerized application using Docker
* Real-time deployment on code push

---
