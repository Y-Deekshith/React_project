pipeline {
    agent 
    { 
        label 'PROD' 
    }
    stages {
        stage('git checkout') {
            steps {
                git 'https://github.com/Y-Deekshith/SnapShot.git'
                sh 'ls -al'
            }
        }
        stage('Install stage') {
            steps {
                sh 'yarn add typescript'
                sh 'yarn install'
                sh 'yarn run test:unit'
            }
        }
        stage('Build stage') {
            steps {
                sh 'yarn run build'
            }
        }
    }
}