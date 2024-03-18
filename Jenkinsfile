/* Requires the Docker Pipeline plugin */
pipeline {
    
    //agent any
    stages {
        stage('checkout') {
            steps {
                //git branch:'main', url: 'https://github.com/cpfarher/jenkins'
                echo "we do not need anymore the checkout"
            }
        }
        stage('build') {
            steps {
                sh 'ls'
            }
        }
        stage('python') {
            agent { docker 'python:3.12.1-alpine3.19' }
            steps {
                sh "python3 --version"
            }
        }
        stage('node'){ 
            agent { docker "node" }
            steps {
                sh "node --version"
            }
        }
    }
}
