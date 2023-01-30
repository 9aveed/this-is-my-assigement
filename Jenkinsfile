pipeline {
    agent any
    stages {
        stage('Build and Push Docker Image') {
            steps {
                sh 'docker login -u naveedalam71 -naveed123456'
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
