pipeline {
    agent any
    stages {

        stage('Build image') {
            steps {
                script {
                    powershell 'docker build --no-cache -t chymaslik/node:test .'
                }
            }
        }
        stage('Deploy image') {
            steps {
                script {
                    powershell '''kubectl delete -f nodeapp.yaml
                    kubectl apply -f nodeapp.yaml'''
                }
            }
        }
    }
}
