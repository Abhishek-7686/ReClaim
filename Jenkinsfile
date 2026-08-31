pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Build') {
            steps {
                echo 'Checking Lost and Found Portal...'
                bat 'dir'
            }
        }

        stage('Test') {
            steps {
                echo 'Running project checks...'
                bat 'if not exist index.html exit /b 1'
            }
        }

        stage('Success') {
            steps {
                echo 'Lost and Found Portal build completed successfully!'
            }
        }
    }
}
