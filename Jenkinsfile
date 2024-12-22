pipeline {
    agent any
    environment {
        CI = 'true'
    }
    stages {
        stage('Setup Node.js') {
            steps {
                sh '''
                    curl -fsSL https://deb.nodesource.com/setup_16.x | bash -
                    sudo apt-get install -y nodejs
                '''
            }
        }
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
