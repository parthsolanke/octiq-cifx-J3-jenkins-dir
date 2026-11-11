pipeline {
    agent any
    stages {
        stage('Test') {
            steps {
                dir('backend') {
                    sh 'npm test'
                }
            }
        }
    }
}
