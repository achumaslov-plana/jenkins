pipeline {
    agent any
    stages {

        stage('Build image') {
        /* This builds the actual image; synonymous to
         * docker build on the command line */
            steps {
                script {
                    bat 'ping 8.8.8.8 -n 2'
                }
            }
        }
    }
}
