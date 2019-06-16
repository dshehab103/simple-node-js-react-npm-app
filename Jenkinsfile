pipeline {
    agent any
    
    tools {nodejs "node"}

    stages {
        stage('Build') {
            steps {
                bat 'npm install'
            }
        }
        stage('Build production file'){
            steps{
                bat 'npm run build'
            }
        }
        
        stage('Test') {
            steps {
                bat 'npm run testecho'
            }
        }

        stage('eject') {
            steps {
                bat 'npm run eject'
            }
        }
        
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}