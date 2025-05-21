pipeline {
    agent any

    stages {
        stage('Build Docker Image') {
            steps {
                sh 'docker build -t abhishekn12/jenkin1 .'
            }
        }
        stage('Run Docker Container') {
            steps {
                sh 'docker run -d  test-container abhishekn12/jenkin1'
            }
        }
    }
}
