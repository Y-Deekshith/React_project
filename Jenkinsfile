pipeline {
    agent any 
    // { 
    //     label 'PROD' 
    // }
    stages {
        stage('git checkout') {
            steps {
                git 'https://github.com/Y-Deekshith/React_project.git'
                sh 'ls -al'
            }
        }
        stage('Build stage') {
            steps {
                sh 'yarn install'
            }
        }
    }
}