pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                echo 'Checking out source code...'
            }
        }

        stage('Build') {
            steps {
                echo 'Building the project...'
                bat 'if exist index.html echo Build successful'
            }
        }

        stage('Test') {
            steps {
                echo 'Testing the project...'
                bat 'if exist index.html (echo Test passed) else (exit /b 1)'
            }
        }

        stage('Finish') {
            steps {
                echo 'CI Pipeline completed successfully!'
            }
        }
    }
}
