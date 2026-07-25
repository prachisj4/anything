pipeline {
    agent any

    parameters {
        choice(
            name: 'ENVIRONMENT',
            choices: ['staging', 'production'],
            description: 'Select deployment environment'
        )
    }

    stages {

        stage('Build') {
            steps {
                echo 'Building...'
            }
        }

        stage('Tests') {
            parallel {

                stage('Unit Tests') {
                    steps {
                        echo 'Running Unit Tests'
                    }
                }

                stage('Integration Tests') {
                    steps {
                        echo 'Running Integration Tests'
                    }
                }

            }
        }

    }
}
