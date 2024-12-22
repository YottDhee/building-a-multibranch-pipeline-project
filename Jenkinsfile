pipeline {
    agent any
    environment {
        CI = 'true'
    }
    stages {
        stage('Build') {
            steps {
                sh 'echo "Build in progress"'
            }
        }
        stage('Test') {
            steps {
                sh 'npm test'
            }
        }
    }
}
