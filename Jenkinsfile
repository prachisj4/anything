
stage('Tests') {
            parallel {
                stage('Unit') {
                    steps {
                        sh 'echo Unit tests'
                    }
                }
                stage('Integration') {
                    steps {
                        sh 'echo Integration tests'
                    }
                }
            }
        }
