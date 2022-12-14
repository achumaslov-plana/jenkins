pipeline {
    agent { docker { image 'stefanscherer/node-windows:latest' } }
    stages {
        stage('build') {
            steps {
                cmd 'node --version'
            }
        }
    }
}
