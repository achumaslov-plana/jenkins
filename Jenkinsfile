pipeline {
    agent none
    stages {
        stage('Build image') {
        /* This builds the actual image; synonymous to
         * docker build on the command line */

            app = docker.build("chymaslik/hellonode")
        }
}
