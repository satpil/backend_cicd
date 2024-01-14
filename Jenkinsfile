pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                script { 
                    checkout scm
                }
            }
        }
        stage('run docker container') {
            steps {
                sh 'docker-compose up'
            }
        }

    }

    post {
        success {
            echo 'Build successful! Send notifications, etc.'
        }

        failure {
            echo 'Build failed! Send notifications, etc.'
        }
    }
}