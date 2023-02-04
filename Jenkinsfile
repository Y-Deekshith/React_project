pipeline {
    agent any 
    // { 
    //     label 'PROD' 
    // }
    stages {
        stage('git checkout') {
            steps {
                git 'https://github.com/Y-Deekshith/SnapShot.git'
                sh 'ls -al'
            }
        }
        stage('Build stage') {
            steps {
                sh 'yarn add typescript'
                sh 'yarn install'
            }
        }
    }
}