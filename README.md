DevOps CI/CD Pipeline Project

 Overview
This project demonstrates a complete CI/CD pipeline that automates the deployment of a containerized application to AWS EC2 using GitHub Actions and Docker.

---

#Architecture

GitHub → GitHub Actions → Docker → AWS EC2 → Nginx → User

---

## ⚙️ Tech Stack

- AWS EC2
- Docker
- GitHub Actions (CI/CD)
- Nginx (Reverse Proxy)
- Flask (Sample Application)

---

## 🚀 Features

- Automated CI/CD pipeline triggered on code push
- Dockerized application for consistent deployment
- Zero manual deployment
- Reverse proxy using Nginx (no port exposure)
- Production-style deployment setup

---

## 📂 Project Structure
devops-pipeline-project/
├── app.py
├── requirements.txt
├── Dockerfile
├── .github/workflows/deploy.yml
└── README.md


---

## 🔄 CI/CD Workflow

1. Developer pushes code to GitHub
2. GitHub Actions triggers pipeline
3. Docker image is built
4. Image transferred to EC2
5. Container deployed automatically

---

## 🌐 Live Demo

👉 http://13.233.25.113
Note: EC2 instance may be stopped to optimize cost. Please contact me to view live demo if unavailable.

---

## 🖥️ How to Run Locally

```bash
git clone <your-repo-url>
cd devops-pipeline-project

pip install -r requirements.txt
python app.py

docker build -t devops-app .
docker run -d -p 5000:5000 devops-app

Deployment is fully automated using GitHub Actions.
Any push to the main branch triggers the pipeline.

## 📸 Screenshots

### ✅ GitHub Actions Pipeline Success
![GitHub Actions](https://github.com/user-attachments/assets/4a225595-0cd0-4880-9c7b-729c4cb3bcc8)

---

### 🐳 Running Docker Container on EC2
![Docker Container](https://github.com/user-attachments/assets/eca51b84-7f0b-4065-9aa9-93e920635ae7)

---

### 🌐 Nginx Reverse Proxy Configuration
![Nginx Config](https://github.com/user-attachments/assets/94488e40-846e-460f-9eaa-92accb5d99c7)


Key Learnings:
CI/CD pipeline implementation
Docker containerization
AWS EC2 deployment
Reverse proxy configuration using Nginx

Author
Yogesh S


