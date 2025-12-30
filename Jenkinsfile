pipeline {
    agent any

    stages {
        stage('Sanity Check') {
            steps {
                echo 'Jenkins pipeline is running'
                sh 'ls'
            }
        }

        stage('Docker Build') {
            steps {
                sh 'docker --version'
                sh 'docker build -t flask-ci-image .'
            }
        }

        stage('Run Container') {
            steps {
                sh '''
                  docker rm -f flask-ci-container || true
                  docker run -d -p 5000:5000 --name flask-ci-container flask-ci-image
                '''
            }
        }
    }
}

