pipeline {
    agent {
        docker { image 'python:3.12-slim' }
    }
    stages {
        stage('Versions') {
            steps {
                sh 'python --version'
                sh 'cat hello.py'
                sh 'python hello.py'
            }
        }
    }
}
