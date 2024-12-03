pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'docker-compose up -d'
            }
        }
        stage('Test') {
            steps {
                sh 'docker exec docker1 ping -c 4 docker2'
            }
        }
    }
}
