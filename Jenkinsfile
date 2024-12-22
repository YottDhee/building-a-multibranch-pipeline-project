pipeline {
    agent any
    tools {
        nodejs 'NodeJS' // Name of the Node.js tool configuration in Jenkins
    }
    stages {
        stage('Build') {
            steps {
                sh 'npm install'
            }
        }
        stage('Test') {
            steps {
                sh 'npm test'
            }
        }
    }
}
