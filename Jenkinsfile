pipeline {
    agent any
    stages {

        stage('Build image') {
            steps {
                script {
                    bat 'docker build -t chymaslik/node:test .'
                }
            }
        }
        stage('Deploy image') {
            steps {
                script {
                    bat 'kubectl apply -f nodeapp.yaml'
                }
            }
        }
    }
}
