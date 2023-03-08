pipeline {
    agent any

    stages {
        stage('checkout') {
            steps {
                checkout scm
            }
        }

        stage('install depedencies') {
            steps {
                sh 'npm install'
            }
        }

        stage('build') {
            steps {
                sh 'ng build -c production'
            }
        }

        stage('deploy') {
            steps {
                sh 'npm start'
            }
        }
    }
}