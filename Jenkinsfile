pipeline {
    environment {
        registry = "hackcoderr/flask:latest" 
        dockerImage = ''
        }
    agent any

    stages {
        stage('Build job') {
            steps { 
                script { 
                    dockerImage = docker.build registry
                }
            } 
        }
    }
}
