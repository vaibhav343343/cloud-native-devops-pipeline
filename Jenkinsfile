pipeline {
    agent any

    stages {

        stage('Clone Code') {
            steps {
                git branch: 'main',
                url: 'https://github.com/vaibhav343343/cloud-native-devops-pipeline.git'
            }
        }

        stage('Install Dependencies') {
            steps {
                sshagent(['ubuntu']) {
                    sh '''
                    ssh -o StrictHostKeyChecking=no ubuntu@3.236.252.74 "
                        cd devops-app
                        source venv/bin/activate
                        pip install -r requirements.txt
                    "
                    '''
                }
            }
        }

        stage('Deploy App') {
            steps {
                sshagent(['ubuntu']) {
                    sh '''
                    ssh -o StrictHostKeyChecking=no ubuntu@3.236.252.74 " 
                        cd devops-app
                        git pull
                        pkill -f app.py || true
                        nohup python3 app.py > log.txt 2>&1 &
                    "
                    '''
                }
            }
        }
    }
}
