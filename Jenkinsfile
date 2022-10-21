pipeline {
    agent any

    stages {
        stage ('Build Docker Image'){
            steps {
                script{
                    dockerapp = docker.build("puppim/kube-new:${env.BUILD_ID}", '-f ./src/Dockerfile ./src')
                }

            }
        }
    }
}