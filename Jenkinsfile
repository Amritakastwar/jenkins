pipeline {
    agent any

    stages {
        stage('Check Workspace') {
            steps {
                echo 'Checking workspace...'
                sh 'ls -la'  // Lists all files in workspace
            }
        }

        stage('Build Test') {
            steps {
                echo 'Running a test build...'
            }
        }

        stage('Hello Jenkins') {
            steps {
                echo 'Jenkins is working!'
            }
        }
    }

    post {
        success {
            echo 'Pipeline finished successfully!'
        }
        failure {
            echo 'Pipeline failed. Check logs!'
        }
    }
}

