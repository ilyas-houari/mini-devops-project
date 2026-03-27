pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                git 'https://github.com/ilyas-houari/mini-devops-project.git'
            }
        }

        stage('Build Docker') {
            steps {
                sh 'docker build -t devops-app .'
            }
        }

        stage('Run') {
            steps {
                sh 'docker-compose up -d'
            }
        }
    }

    post {
        success {
            echo 'Build success'
        }
        failure {
            echo 'Build failed'
        }
    }
}