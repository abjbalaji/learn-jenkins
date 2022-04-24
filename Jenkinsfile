pipeline {
    agent any
    environment{
    ENV_VAR="pipeline.google.in"
    }
    stages {
        stage('Build') {
            steps {
                sh'''
                echo Environment var is ${ENV_VAR}
                echo Building...
                '''
            }
        }
        stage('Test') {
            steps {
                echo 'Testing...'
            }
        }
        stage('Deploy') {
        
            steps {
                echo 'Environment is =${ENV_VAR}...'
            }
        }
    }
}