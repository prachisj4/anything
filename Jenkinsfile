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
    }
}
