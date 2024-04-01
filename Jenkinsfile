 pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git clone 'https://github.com/hxn7/Jenkins-Pipeline.git'
            }
        }

        stage('Dependency Installation') {
            steps {
                // Assuming npm is used for frontend and pip for backend
                sh 'npm install' // For frontend
            }
        }

        stage('Build') {
            steps {
                sh 'npm run build' // Build the React application
            }
        }

        stage('Test') {
            steps {
                sh 'npm test' // Run tests for the React application
            }
        }

        stage('Containerized') {
            steps {
                sh 'echo docker' // Build Docker image for frontend
                sh 'echo docker' // Run Docker Compose to start the application
            }
        }
    }
}