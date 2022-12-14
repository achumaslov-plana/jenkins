pipeline {
    agent none
    stages {
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
