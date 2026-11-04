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
    }
}
