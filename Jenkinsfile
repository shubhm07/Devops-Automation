pipeline {
    agent any
    tools{
        maven 'maven_3_8_6'
    }
    stages{
        stage('Build Maven'){
            steps{
#                checkout([$class: 'GitSCM', branches: [[name: '*/master']], extensions: [], userRemoteCogit addnfigs: [[url: 'https://github.com/shubhm07/Devops-Automation']]])
                bat 'mvn -Dplugin=install help:describe'
            }
        }
    }
}