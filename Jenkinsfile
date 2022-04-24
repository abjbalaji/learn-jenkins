pipeline {
    agent any
    environment{
    USER_CRED= credentials("SSH")
    }

    stages {
        stage('Hello') {
            steps {
                sh 'env'

            }
        }
    }
}
