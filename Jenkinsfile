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
            }
        }
        stage('Build stage') {
            steps {
                sh 'yarn run build'
            }
        }
        stage('start stage') {
            steps {
                sh 'yarn start'
                sh 'sleep 30'
                sh 'exit'
            }
        }
    }
}