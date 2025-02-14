pipeline {
    agent any

    stages {
        stage('NPM Install') {
            steps {
                sh '/bin/sh -c "npm install"'
            }
        }
        stage('Run Integration Tests') {
            steps {
                sh '/bin/sh -c "npm run test"'
            }
        }
    }
}
