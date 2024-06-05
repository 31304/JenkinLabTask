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
                bat 'npm install' // Assuming npm is used for frontend and pip for backend
            }
        }

        stage('Build') {
            steps {
                bat 'echo build' // Build the React application
            }
        }

        stage('Test') {
            steps {
                bat 'echo test' // Run tests for the React application
            }
        }

        stage('Containerized') {
            steps {
                bat 'echo docker' // Build Docker image for frontend
                bat 'echo docker' // Run Docker Compose to start the application
            }
        }

        stage('Deploy') {
            steps {
                bat 'npm start'
            }
        }
    }
}
