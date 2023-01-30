

pipeline {
    stages {
        stage('Build and Push Docker Image') {
            steps {
                sh 'docker login -u naveedalam71 -p kabeer@125'
                sh 'docker-compose build'
                sh 'docker-compose push'
            }
        }
        stage('Push Docker Image') {
            steps {
                sh 'docker-compose push'
                }
        }
    }
}
