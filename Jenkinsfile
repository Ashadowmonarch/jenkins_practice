pipeline {
    agent {
        docker { image 'python:3.10' }
    }
    stages {
        stage('Clone Repository') {
            steps {
                git branch: 'main', url: 'https://github.com/Ashadowmonarch/jenkins_practice.git'
            }
        }
        stage('Run Python Script') {
            steps {
                sh 'python main.py'
            }
        }
    }
}
