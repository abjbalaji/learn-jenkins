pipeline {
    agent any

   parameters {
           string(name: 'PERSON', defaultValue: 'Mr Jenkins', description: 'Who should I say hello to?')

           text(name: 'BIOGRAPHY', defaultValue: '', description: 'Enter some information about the person')

           booleanParam(name: 'TOGGLE', defaultValue: true, description: 'Toggle this value')

           choice(name: 'CHOICE', choices: ['One', 'Two', 'Three'], description: 'Pick something')

           password(name: 'PASSWORD', defaultValue: 'SECRET', description: 'Enter a password')
    }

    tools {
    maven 'maven-3.6.3'
    }
    stages {
        stage('Hello') {
            input {
                            message "Should we continue?"
                            ok "Yes, we should."
                            submitter "alice,bob"
                            parameters {
                                string(name: 'PERSON', defaultValue: 'Mr Jenkins', description: 'Who should I say hello to?')
                            }
                        }
            steps {

                echo "hello gjoljfklgjrfgkljro are you"
                sh 'mvn --version'
            }
        }
    }
}
