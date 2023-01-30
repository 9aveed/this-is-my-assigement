pipeline {
    agent any
    stages {
        stage('Build and Push Docker Image') {
            steps {
                sh 'echo "naveed12345" | docker login -u naveedalam71 --password-stdin'
                sh 'docker-compose build'
            }
        }
        stage('Push Docker Image') {
            steps {
                sh 'docker-compose push'
                }
        }
    }
}
