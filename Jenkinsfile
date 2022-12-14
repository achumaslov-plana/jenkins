pipeline {
    agent any
    stages {
        stage('Cloning Git') {
            steps {
                git 'https://github.com/achumaslov-plana/jenkins.git'
            }
        }
        stage('Build image') {
        /* This builds the actual image; synonymous to
         * docker build on the command line */
            steps {
                script {
                    sh 'docker build -t chymaslik/test:latest .'
                }
            }
        }
    }
}
