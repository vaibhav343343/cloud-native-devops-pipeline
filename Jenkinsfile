pipeline {
    agent any

    stages {
        stage('Build Docker Image') {
            steps {
                sh 'docker build -t flask-devops-app .'
            }
        }

        stage('Run Docker Container') {
            steps {
                sh '''
                docker rm -f flask-devops-container || true
                docker run -d -p 5000:5000 --name flask-devops-container flask-devops-app
                '''
            }
        }
    }
}
