pipeline {
    agent any
    stages {
        stage('Pre-build') {
            steps {
                bat 'echo Pre-build'
            }
        }
        stage('Build') {
            steps {
                bat 'echo Build in progress.'
            }
        }
        stage('Unit tests') {
            steps {
                bat 'echo Running unit tests'
            }
        }
        stage('Deploy') {
            steps {
                bat 'echo Deploying build'
            }
        }
        stage('Regression tests') {
            parallel {
                stage('Chrome') {
                    steps {
                        bat 'echo Running E2E tests on Chrome'
                        // Add actual commands for running E2E tests on Chrome
                    }
                }
                stage('Firefox') {
                    steps {
                        bat 'echo Running E2E tests on Firefox'
                        // Add actual commands for running E2E tests on Firefox
                    }
                }
                stage('Safari') {
                    steps {
                        bat 'echo Running E2E tests on Safari'
                        // Add actual commands for running E2E tests on Safari
                    }
                }
            }
        }
        stage('Release to prod') {
            steps {
                bat 'echo Releasing to prod'
            }
        }
    }
    post {
        always {
            echo 'Cleanup after everything!'
        }
    }
}
