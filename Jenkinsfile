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

            }
        }
        
        stage('Test') {
            steps {
                // Perform testing steps here
                sh 'echo "release v.2"'
                sh 'pwd'
                sh 'ls'
            }
        }
        
    }
}
