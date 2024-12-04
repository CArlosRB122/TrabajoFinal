pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                bat 'my-windows-command'  // Ejecutar tu comando en Windows
            }
        }
        stage('Test') {
            steps {
                // Reemplazamos 'sh' por 'bat' y ajustamos el comando ping para Windows
                bat 'docker exec docker1 ping -n 4 docker2'
            }
        }
    }
}
