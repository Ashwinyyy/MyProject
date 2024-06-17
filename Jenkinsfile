pipeline {
    agent any
    stages {
        stage('Pre-build') {
            steps {
                sh 'echo Pre-build'
            }
        }
        stage('Build') {
            steps {
                sh 'echo Build in progress.'
            }
        }
        stage('Unit tests') {
            steps {
                sh 'echo Running unit tests'
            }
        }
        stage('Deploy') {
            steps {
                sh 'echo Deploying build'
            }
        }
        stage('Regression tests') {
            parallel {
                stage('Chrome') {
                    steps {
                        sh 'echo Running E2E tests on Chrome'
                    }
                }
                stage('Firefox') {
                    steps {
                        sh 'echo Running E2E tests on Firefox'
                    }
                }
                stage('Safari') {
                    steps {
                        sh 'echo Running E2E tests on Safari'
                    }
                }
            }
        }
        stage('Release to prod') {
            steps {
                sh 'echo Releasing to prod'
            }
        }
    }
    post {
        always {
            echo 'Cleanup after everything!'
        }
    }
}
