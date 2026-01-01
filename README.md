🚀 Cloud-Native DevOps Pipeline (Jenkins + Docker + AWS)
📌 Project Overview
This project demonstrates a real-time cloud-native CI/CD pipeline using Jenkins, Docker, and AWS EC2.
A Flask web application is containerized using Docker and automatically built and deployed through a Jenkins pipeline.

The application is exposed publicly via AWS EC2 Security Groups and runs inside a Docker container.


🛠️ Tech Stack
Cloud: AWS EC2 (Ubuntu)

CI/CD: Jenkins

Containerization: Docker

Application: Python Flask

Version Control: Git & GitHub


🧩 Architecture Flow
Developer pushes code to GitHub

Jenkins pulls the repository

Docker image is built from Dockerfile

Container is deployed on AWS EC2

Flask app is exposed on port 5000


📂 Project Structure
cloud-native-devops-pipeline/
│
├── app.py          # Flask application
├── Dockerfile      # Docker image configuration
├── Jenkinsfile     # Jenkins CI/CD pipeline
└── README.md       # Project documentation
🐍 Flask Application
A simple Flask app that confirms successful deployment.

Output:  Flask app is running successfully!


🐳 Docker Configuration
Uses python:3.10-slim base image

Exposes port 5000

Runs Flask app using Python


⚙️ Jenkins Pipeline Stages
Clone GitHub repository

Build Docker image

Run Docker container

Expose application


🌐 Live Application Access
After successful deployment, access the application using:

http://<EC2_PUBLIC_IP>:5000
Example: http://18.207.100.244:5000


🔐 AWS Security Group Rules
Port	Protocol	Source
22	TCP	SSH
5000	TCP	0.0.0.0/0


✅ Features
End-to-end CI/CD pipeline

Dockerized application

Cloud deployment on AWS

Real-time public access

Resume & internship ready project



📈 Future Improvements
Add Nginx reverse proxy

Use Docker Compose

Deploy using Kubernetes

Add monitoring with Prometheus & Grafana



👨‍💻 Author
Vaibhav Sudrik
Cloud Computing & DevOps Enthusiast 🚀


⭐ GitHub
If you like this project, don’t forget to ⭐ the repository!
