pipeline {
    agent any

    stages {
        stage('NPM Install') {
            steps {
                bat 'npm install'
            }
        }
        stage('Run Integration Tests') {
            steps {
                bat 'npm run test'
            }
        }
    }
}