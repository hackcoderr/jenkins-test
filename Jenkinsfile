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
        stage('Test Job') {
            steps {
                echo 'Test Job'
                sleep 10
            }
        }
        stage('Deploy Job') {
            steps {
                echo 'Deploy Job'
                sleep 10
            }
        }
    }
}
