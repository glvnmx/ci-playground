pipeline {
    agent {
        docker { image 'python:3.12-slim' }
    }
    stages {
        stage('Lint (ruff)') {
            steps {
                sh 'python -m venv .venv'
                sh '.venv/bin/pip install --no-cache-dir ruff'
                sh '.venv/bin/ruff --version'
                sh '.venv/bin/ruff check .'
            }
        }
    }
}
