pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/Radhay-raman/jenkins-ci-demo.git'
            }
        }

        stage('Build') {
            steps {
                echo 'No build required'
            }
        }

        stage('Test') {
            steps {
                bat 'pytest'
            }
        }
    }
}
