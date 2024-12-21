pipeline {
    agent {
        docker { image 'python:3.10' } // Use a Python Docker image
    }
    stages {
        stage('Clone Repository') {
            steps {
                // Clone the GitHub repository
                git branch: 'main', url: 'https://github.com/Ashadowmonarch/jenkins_practice.git'
            }
        }
        stage('Run Python Script') {
            steps {
                // Run your Python script
                sh 'python main.py'
            }
        }
    }
}
