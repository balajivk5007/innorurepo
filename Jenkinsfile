pipeline {
    agent any
    stages {
        stage('Clone Repository') {
            steps {
                git url: 'https://github.com/balajivk5007/innorurepo.git'
            }
        }
        stage('Install Dependencies') {
            steps {
                bat 'npm install'
            }
        }
        stage('Run Application') {
            steps {
                bat 'node work.js'
            }
        }
    }
    post {
        always {
            echo 'Pipeline completed.'
        }
    }
}