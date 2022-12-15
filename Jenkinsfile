pipeline {
    agent any
    stages {

        stage('Build image') {
            steps {
                script {
                    powershell 'docker build -t chymaslik/node:test .'
                }
            }
        }
        stage('Deploy image') {
            steps {
                script {
                    powershell 'kubectl apply -f nodeapp.yaml'
                }
            }
        }
    }
}
