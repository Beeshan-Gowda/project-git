pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git url: 'https://github.com/Beeshan-Gowda/project-git'
            }
        }

        stage('Build') {
            steps {
                echo 'Building...'
                // sh 'make'
            }
        }

        stage('Test') {
            steps {
                echo 'Testing...'
                // 'make test'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying...'
                // sh 'make deploy'
            }
        }
    }

    post {
        success {
            echo 'Pipeline completed successfully!'
        }
        failure {
            echo 'Pipeline failed!'
        }
    }
}
