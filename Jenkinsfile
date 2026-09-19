pipeline {
    agent any
    stages {
        stage('Test') {
            steps {
                sh 'python3 -m venv venv'
                sh '. venv/bin/activate && pip install pytest'
                sh '. venv/bin/activate && pytest'
            }
        }
    }
}
