pipeline {
    agent any

    stages {
        stage('Build Docker Image') {
            steps {
                sh 'docker build -t jenkin1 .'
            }
        }
        stage('Run Docker Container') {
            steps {
                sh 'docker run -d --name test-container jenkin1'
            }
        }
    }
}
