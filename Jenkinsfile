/* Requires the Docker Pipeline plugin */
pipeline {
    //agent { docker { image 'python:3.12.1-alpine3.19' } }
    agent any
    stages {
        stage('checkout') {
            steps {
                git branch:'main', url: 'https://github.com/cpfarher/jenkins'
            }
        }
        stage('build') {
            steps {
                sh 'ls'
            }
        }
    }
}
