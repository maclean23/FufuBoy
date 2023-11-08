pipeline {
    agent any

    stages {
        stage('compile') {
            steps {
                echo 'compilng stage'
                git branch: 'main', url: 'git@github.com:maclean23/FufuBoy.git'
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
                echo 'package stage'
                sh 'mvn package'
            }
        }
        stage('move to dockerfile') {
            steps {
                echo 'creating dockerfile'
                sh 'touch dockerfile'
            }
        }
    }
}
