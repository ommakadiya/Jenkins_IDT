pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo 'Checking out source code...'
                checkout scm
            }
        }

        stage('Build') {
            steps {
                echo 'Building the project...'
                sh 'test -f index.html'
                echo 'Build successful'
            }
        }

        stage('Test') {
            steps {
                echo 'Testing the project...'
                sh 'test -f index.html'
                echo 'Test passed'
            }
        }

        stage('Finish') {
            steps {
                echo 'CI Pipeline completed successfully!'
            }
        }
    }
}
