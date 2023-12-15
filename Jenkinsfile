pipeline {
    agent { docker { image 'python:3.7.2' } }
    stages {
        stage('build') {
            steps {
                sh '''
                python3 -m venv env &&
                source env/bin/activate &&
                pip install flask
                '''
            }
        }
        stage('test') {
            steps {
                sh '''
                source env/bin/activate &&
                python test.py
                '''
            }
        }
    }
}
