pipeline {
    agent any

    stages {
        stage ('Build Docker Image') {
            steps {
                script {
                    dockerapp = docker.build("wsrfreitas/kube-news:${env.BUILD_ID}", '-f ./scr/Dockerfile ./src')
                }
            }
        }
    }
}