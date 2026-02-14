pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'No build required'
            }
        }

        stage('Setup Python Environment') {
            steps {
                bat 'python -m venv venv'
                bat 'venv\\Scripts\\pip install --upgrade pip'
                bat 'venv\\Scripts\\pip install pytest'
            }
        }

        stage('Test') {
            steps {
                bat 'venv\\Scripts\\python -m pytest'
            }
        }
    }
}
