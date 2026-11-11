pipeline {
    agent any

    stages {

        stage('AWS Identity Check') {

            steps {

                withCredentials([
                    string(credentialsId: 'aws-access-key', variable: 'AWS_ACCESS_KEY_ID'),
                    string(credentialsId: 'aws-secret-key', variable: 'AWS_SECRET_ACCESS_KEY')
                ]) {

                    sh '''
                        export AWS_DEFAULT_REGION=us-east-1
                        aws sts get-caller-identity
                    '''
                }
            }
        }
    }
}
