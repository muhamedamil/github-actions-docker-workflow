# 🚀 GitHub Actions + Docker CI/CD Demo

This project is a **demo application** that demonstrates how to automate an **end-to-end CI/CD pipeline** using **GitHub Actions** and **Docker**.  
The workflow covers **containerization**, **automated builds**, and **deployment to Docker Hub**.

---

## 📌 Features
- GitHub Actions workflow for **automated builds**.
- **Docker containerization** for consistent environments.
- **Automatic image push** to Docker Hub on every commit to `main`.
- Simple demo application to test the pipeline.
- Clean and scalable project structure.

---

## 🛠️ Tech Stack
- **GitHub Actions** – Workflow automation
- **Docker** – Containerization and image management
- **Python** (Flask or FastAPI) – Demo application
- **Docker Hub** – Deployment target

---

## ⚙️ Workflow Overview
Below is the process automated by GitHub Actions:

1. **Code pushed to GitHub** → triggers the workflow.
2. GitHub Actions **builds the Docker image**.
3. Workflow **pushes the image to Docker Hub**.
4. Docker image can then be **pulled and run anywhere**.

---

## 📂 Project Structure

.
├── app/
│   ├── main.py           # Demo application code
│   └── requirements.txt  # Python dependencies
├── Dockerfile            # Docker image build instructions
├── .github/
│   └── workflows/
│       └── ci-cd.yml     # GitHub Actions workflow
└── README.md


## 🚢 Docker Workflow

### **1. Build Docker Image Locally**
```bash
docker build -t your-dockerhub-username/demo-app .

## Run the Container :
docker run -d -p 8000:8000 your-dockerhub-username/demo-app

## Push Image to Docker Hub
