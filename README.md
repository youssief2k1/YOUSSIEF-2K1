# DevOps CI/CD Project

## 🚀 Overview
This project demonstrates a complete **DevOps pipeline** using **Jenkins**, **Docker**, and **Terraform** to build, test, deploy, and monitor a web application on an **AWS EC2 instance**.

The application is containerized using Docker and automatically deployed through a Jenkins pipeline, showcasing skills in automation, cloud deployment, and CI/CD best practices.

---

## 🧰 Technologies Used
- **Jenkins** – CI/CD automation
- **Docker** – Containerization
- **Terraform** – Infrastructure as Code (IaC)
- **Python / Flask** – Web Application
- **AWS EC2** – Deployment environment
- **GitHub Actions** – Workflow automation
- **Prometheus & Grafana** – Monitoring and visualization

---

## 📁 Project Structure
```
YOUSSIEF-2K1/
├── app/                  # Flask application source code
├── monitoring/           # Prometheus and Grafana setup
├── systemd/              # Service configuration files
├── terraform/            # IaC scripts for AWS EC2 deployment
├── tests/                # Unit tests
├── Dockerfile            # Build instructions for Docker image
├── docker-compose.yml    # Multi-container configuration
├── requirements.txt      # Python dependencies
├── Jenkinsfile           # Jenkins CI/CD pipeline
└── .github/workflows/    # GitHub Actions workflows
```

---

## ⚙️ How to Run Locally

### 1️⃣ Build and Run with Docker
```bash
docker build -t flask-app .
docker run -d -p 8080:80 flask-app
```

Then open in browser:  
👉 [http://localhost:8080](http://localhost:8080)

---

## 🧩 Jenkins Pipeline
The **Jenkinsfile** defines the following stages:

1. **Build** – Build the Docker image  
2. **Test** – Run automated tests  
3. **Push** – Push the image to DockerHub  
4. **Deploy** – Deploy to EC2 using Terraform  

To trigger the pipeline:
- Connect Jenkins to this repository via Webhook.
- Run the pipeline manually or automatically on every commit.

---

## 🖼️ Screenshots
- ✅ Jenkins Pipeline Successful Run  
- ✅ Running Container on EC2 Instance  
- ✅ Application accessed via Public IP  

(Add your screenshots here)

---

## 👨‍💻 Author
**Youssief Abdelghany Mohamed**  
DevOps Engineer | Cloud & Automation Enthusiast  
[GitHub Profile](https://github.com/youssief2k1)
