/* Requires the Docker Pipeline plugin */
pipeline {
    agent { docker 'python:3.12.1-alpine3.19' }
    //agent any
    stages {
        stage('checkout') {
            steps {
                //git branch:'main', url: 'https://github.com/cpfarher/jenkins'
                echo 'we do not need anymore the checkout'
            }
        }
        stage('build') {
            steps {
                sh 'ls'
            }
        }
        stage('python') {
            steps {
                sh "python3 --version"
            }
        }
    }
}
