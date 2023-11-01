pipeline {
    agent any

    stages {
        stage('compile') {
            steps {
                echo 'compile stage'
                git branch: 'main', url: 'https://github.com/maclean23/FufuBoy.git'
                sh 'mvn compile'
            }
        }
        stage('test') {
            steps {
                echo 'testing stage'
                sh 'mvn test'
            }
        }
        stage('package') {
            steps {
                echo 'package'
                sh 'mvn package'
            }
        }
        stage('Publish to Nexus') {
            steps {
                echo 'Publishing artificat'
            }
        }
        stage('Aqua-scan') {
            steps {
                echo 'scanning for security'
            }
        }
        stage('Docker-build') {
            steps {
                echo 'Creating image'
            }
        }
        stage('Push image to dockerhub') {
            steps {
                echo 'pushing image to dockerhub'
            }
        }
        stage('Deploy on Dev Enviornment') {
            steps {
                echo 'Deploying on Dev enviornment'
            }
        }
        stage('Deploy on Pre-Prod Enviornment') {
            steps {
                echo 'Deploying on pre-prod environment'
            }
        }
        stage('Deploy on Prod Enviornment') {
            steps {
                echo 'Deploying on production enviornment'
                
            }
        }
    
    }
}    
