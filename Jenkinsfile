pipeline {
    agent any

    stages {

        stage('Server Info') {
            steps {
                sh '''
                whoami
                pwd
                hostname
                date
                '''
            }
        }

        stage('Disk Usage') {
            steps {
                sh 'df -h'
            }
        }
    }
}
