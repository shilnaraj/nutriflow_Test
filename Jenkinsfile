pipeline {
    agent any

    stages {
        stage('Build Backend') {
            steps {
                bat '''
                    cd backend
                    npm install
                '''
            }
        }

        stage('Build Frontend') {
            steps {
                bat '''
                    cd frontend
                    npm install
                    npm run build
                '''
            }
        }
    }
}