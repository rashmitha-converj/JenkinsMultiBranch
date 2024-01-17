pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                nodejs('nodejs') {
                    sh 'node -v'
                    sh 'npm -v'
                    sh 'ls'
                    sh 'npm install'
                    sh 'npm start &'
                }
            }
        }
    }
}
