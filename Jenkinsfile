pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo 'Checking out code...' // test webhook
                checkout scm
            }
        }
        stage('Build') {
            steps {
                echo 'Building the project...'
                sh 'echo "Build step running"'
            }
        }
        stage('Test') {
            steps {
                echo 'Running tests...'
                sh 'echo "Test step running"'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying application...'
                sh 'echo "Deploy step running"'
            }
        }
    }

    post {
        success {
            echo 'Pipeline succeeded!'
        }
        failure {
            echo 'Pipeline failed!'
        }
    }
}
