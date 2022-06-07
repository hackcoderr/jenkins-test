pipeline {
    environment {
        registry = "hackcoderr/flask:latest" 
        registryCredential = 'dockercred'
        dockerImage = ''
        }
    agent{
        label 'docker-node'
    }

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
