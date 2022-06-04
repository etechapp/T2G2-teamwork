pipeline {
    agent any
    stages {
        stage ('Git-Clone') {
            steps {
               checkout([$class: 'GitSCM', branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[credentialsId: 'GitHubCredentials', url: 'https://github.com/etechapp/T2G2-teamwork.git']]]) 
            }
        }
        stage ('1-chidany') {
            steps {
                sh 'lscpu'
                sh 'echo $SHELL'
            }
        }
        stage ('2-mike') {
            steps {
                sh 'ps -ef'
                sh 'systemctl status jenkins'
            }
        }
        stage ('3-saada') {
            steps{
                sh 'free -g'
                sh 'echo In this group no one will be left behind'
            }
        }
        stage('4-monic') {
            steps{
                sh 'df -h'
                sh 'scp'
            }
        }
    }
}
