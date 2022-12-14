pipeline {
    agent { docker { image 'stefanscherer/node-windows:latest' } }
    stages {
        stage('build') {
            steps {
                sh 'node --version'
            }
        }
    }
}
