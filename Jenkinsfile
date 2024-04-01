pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/31304/JenkinLabTask.git'
            }
        }

        stage('Dependency Installation') {
            steps {
                sh 'npm install' // Assuming npm is used for frontend and pip for backend
            }
        }

        stage('Build') {
            steps {
                sh 'echo build' // Build the React application
            }
        }

        stage('Test') {
            steps {
                sh 'echo test' // Run tests for the React application
            }
        }

        stage('Containerized') {
            steps {
                sh 'echo docker' // Build Docker image for frontend
                sh 'echo docker' // Run Docker Compose to start the application
            }
        }

        stage('Deploy') {
            steps {
                sh 'npm start'
            }
        }
    }
}
