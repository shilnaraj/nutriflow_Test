pipeline {
    agent any

    stages {

        stage('Backend - Install') {
            steps {
                bat 'cd backend && npm ci'
            }
        }

        stage('Frontend - Install') {
            steps {
                bat 'cd frontend && npm ci'
            }
        }

        stage('Frontend - Build') {
            steps {
                bat 'cd frontend && npm run build'
            }
        }
    }
}