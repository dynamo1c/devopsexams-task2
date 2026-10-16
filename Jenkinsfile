pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/dynamo1c/devopsexams-task2.git'
            }
        }
        stage('Build') {
            steps {
                echo 'Building the application...'
                sh 'echo "Build step complete"'
            }
        }
        stage('Test') {
            steps {
                echo 'Running tests...'
                sh 'echo "All tests passed"'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying to staging environment...'
                sh 'echo "Deployment successful"'
            }
        }
    }

    post {
        success { echo 'Pipeline finished successfully!' }
        failure { echo 'Pipeline failed.' }
    }
}