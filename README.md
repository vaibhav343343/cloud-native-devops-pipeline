# Cloud-Native DevOps Pipeline

![CI/CD](https://img.shields.io/badge/CI%2FCD-Jenkins-blue)
![Docker](https://img.shields.io/badge/Docker-Containerized-blue)
![AWS](https://img.shields.io/badge/AWS-EC2-orange)
![Python](https://img.shields.io/badge/Python-Flask-green)

End-to-end CI/CD pipeline using Jenkins, Docker, and AWS EC2.

---

## Overview
This project demonstrates an automated CI/CD pipeline where a Flask application is built,
containerized, and deployed on AWS EC2 using Jenkins.

---

## Architecture
GitHub → Jenkins → Docker → AWS EC2 → Flask Application
## Architecture


---

## CI/CD Workflow
1. Source code pushed to GitHub
2. Jenkins pipeline triggered
3. Docker image built
4. Docker container deployed on EC2
5. Application exposed via public IP

---

## Project Structure
cloud-native-devops-pipeline/
├── app.py
├── Dockerfile
├── Jenkinsfile
├── README.md
└── .gitignore

---

## Docker Commands
docker build -t flask-ci-image .
docker run -d -p 5000:5000 flask-ci-image

---

## Live Application
http://<EC2_PUBLIC_IP>:5000


---

## Key Learnings
- Jenkins CI pipelines
- Docker containerization
- AWS EC2 deployment
- Security group configuration

---

## Author
Vaibhav Sudrik  
Cloud Computing Student | DevOps Enthusiast
