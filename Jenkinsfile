pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building the app...'
                sh 'npm install'
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
                sh 'npm test || true'
            }
        }

        stage('Docker Build and Run') {
            steps {
                echo 'Building Docker image...'
                sh 'docker build -t my-node-app .'

                echo 'Running container...'
                sh 'docker run -d -p 3000:3000 my-node-app'
            }
        }
    }
}
