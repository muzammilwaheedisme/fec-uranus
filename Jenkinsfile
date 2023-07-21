pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'npm install'
                sh 'npm run start'
                sh 'npm run server-prod'
            }
        }
        stage('Test') {
            steps {
                sh 'npm run test'
            }
        }
    }
}