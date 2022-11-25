pipeline {
    agent any
    stages{
        stage('Build Maven'){
            steps{
                checkout([$class: 'GitSCM', branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/shubhm07/Devops-Automation']]])
                sh 'mvn clean install'
            }
        }
    }
}