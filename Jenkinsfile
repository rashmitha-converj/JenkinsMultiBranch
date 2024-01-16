// Install DockerPipeline Plugin
// usermod -aG docker jenkins
// restart jenkins url:8080/restart

// pipeline {
//     agent none

//     stages {
//         stage('Build') {
//             agent {
//                 docker {
//                     image 'node:16'
//                 }
//             }
//             steps {
//                 // Perform build steps here
//                 sh 'echo "first step"'
//                 sh 'node -v'
//                 sh 'pwd'
//                 sh 'touch test.js'
//                 sh 'ls'

//             }
//         }
        
//         stage('Test') {
//             agent {
//                 docker {
//                     image 'python:latest'
//                 }
//             }
//             steps {
//                 // Perform testing steps here
//                 sh 'echo "second step"'
//                 sh 'pwd'
//                 sh 'ls'
//             }
//         }
        
//     }
// }

pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                // Perform build steps here
                sh 'echo "first step"'
                sh 'pwd'
                sh 'touch test.js'
                sh 'ls'
                sh 'whoami'
                sh 'curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.1/install.sh | bash'
                sh 'export NVM_DIR="$HOME/.nvm"'
                    sh 'ls /usr/local/bin'
                    sh 'ls /usr/bin'
                sh 'npm install'
                sh 'npm start'

            }
        }
        
        stage('Test') {
            steps {
                // Perform testing steps here
                sh 'echo "branch dev"'
                sh 'pwd'
                sh 'ls'
            }
        }
        
    }
}
