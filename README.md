\# Cloud-Native DevOps Pipeline (Jenkins, Docker, AWS)



\## Overview

This project demonstrates an end-to-end CI/CD pipeline using Jenkins, Docker, and AWS EC2.

A Flask web application is containerized using Docker and automatically built and deployed via Jenkins.



\## Architecture

\- Source Control: GitHub

\- CI/CD Tool: Jenkins

\- Containerization: Docker

\- Cloud Platform: AWS EC2 (Ubuntu)

\- Application: Python Flask





\## CI/CD Workflow

1\. Code pushed to GitHub

2\. Jenkins pipeline triggered

3\. Docker image built

4\. Docker container deployed on EC2

5\. Application exposed via public IP





\## Project Structure

cloud-native-devops-pipeline/

├── app.py

├── Dockerfile

├── Jenkinsfile

├── README.md

└── .gitignore





\## Docker Commands

docker build -t flask-ci-image .

docker run -d -p 5000:5000 flask-ci-image





\## Jenkins Pipeline

\- Checkout source code

\- Build Docker image

\- Run Docker container





\## Live Application

http://<EC2\_PUBLIC\_IP>:5000





\## Key Learnings

\- Jenkins CI pipeline

\- Docker build \& run

\- AWS EC2 deployment

\- Security group configuration





\## Author

Vaibhav Sudrik  

Cloud Computing Student | DevOps Enthusiast



