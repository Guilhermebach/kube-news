pipeline {
    agent any

    stages {
        stage ('Build Docker Image') {
            steps {
                script {
                    dockerapp = docker.build("bach93/kubenews:${env.BUILD_ID}", '.')
                }
            }
        }
    }
}