pipeline {
    agent any

    stages {
        stage('Build Docker Image') {
            steps {
                sh 'docker build -t my-test-image .'
            }
        }
        stage('Run Docker Container') {
            steps {
                sh 'docker run -d --name test-container my-test-image'
            }
        }
    }
}
