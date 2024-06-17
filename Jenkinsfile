pipeline {
    agent any
    stages {
        stage('Parallel Stage') {
            parallel {
                stage('Stage 1') {
                    steps {
                        echo 'Executing Stage 1'
                        // Add any commands or steps you want to run in Stage 1
                    }
                }
                stage('Stage 2') {
                    steps {
                        echo 'Executing Stage 2'
                        // Add any commands or steps you want to run in Stage 2
                    }
                }
            }
        }
    }
}
