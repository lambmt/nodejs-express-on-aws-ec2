pipeline {
    agent {
        label 'slave2'
    }
     environment {
            CI = 'true'
        }
    stages {
        stage('Build') {
            steps {
                sh 'npm install'
            }
        }
        stage('Test') {
            steps {
                sh 'node app.js'
            }
        }      
    }
}