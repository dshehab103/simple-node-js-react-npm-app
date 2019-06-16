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

        stage('test1') {
            steps {
                bat 'npm run  --env=jsdom'
            }
        }
        
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}