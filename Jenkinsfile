pipeline {
    agent any
    tools{
        maven 'maven_3_5_0'
    }
    stages{
        stage('Build Maven'){
            steps{
                checkout([$class: 'GitSCM', branches: [[name: '*/master']], extensions: [], userRemoteCogit addnfigs: [[url: 'https://github.com/shubhm07/Devops-Automation']]])
                sh 'mvn clean install'
            }
        }
    }
}