pipeline {
    agent any
    environment{
    USER_CRED= credentials("SSH")
   parameters {
           string(name: 'PERSON', defaultValue: 'Mr Jenkins', description: 'Who should I say hello to?')

           text(name: 'BIOGRAPHY', defaultValue: '', description: 'Enter some information about the person')

           booleanParam(name: 'TOGGLE', defaultValue: true, description: 'Toggle this value')

           choice(name: 'CHOICE', choices: ['One', 'Two', 'Three'], description: 'Pick something')

           password(name: 'PASSWORD', defaultValue: 'SECRET', description: 'Enter a password')
    }
    triggers {
        cron('* * * * *')
         }
    stages {
        stage('Hello') {
            steps {
                sh 'env'
                echo 'hello how are you'

            }
        }
    }
}
