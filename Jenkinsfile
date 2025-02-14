pipeline {
    agent any

    environment {
        PATH = "/opt/homebrew/bin:/usr/local/bin:/usr/bin:/bin:/usr/sbin:/sbin"
    }

    stages {
        stage('NPM Install') {
            steps {
                sh 'npm install'
            }
        }
        stage('Run Integration Tests') {
            steps {
                sh 'npm run test'
            }
        }
        stage('Run NPM Audit Tests') {
            steps {
                sh 'npm audit'
            }
        }
    }
}
