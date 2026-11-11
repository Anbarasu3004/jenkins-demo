pipeline {
    agent any

    stages {

        stage('Credentials Test') {

            steps {

                withCredentials([
                    usernamePassword(
                        credentialsId: 'github-demo',
                        usernameVariable: 'USER',
                        passwordVariable: 'PASS'
                    )
                ]) {

                    sh '''
                    echo "Username is: $USER"
                    '''
                }
            }
        }
    }
}
