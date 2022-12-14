pipeline {
    agent any
    stages {
        stage('Cloning our Git') {
            steps {
                git 'https://github.com/YourGithubAccount/YourGithubRepository.git'
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
