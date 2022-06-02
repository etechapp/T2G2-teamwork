pipeline {
    agent any
    stages {
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
    }
}
