pipeline {
    agent any
    stages {
        stage('Test') {
            steps {
                sh '''
                    python3 -m venv venv
                    . venv/bin/activate
                    python3 -m ensurepip --upgrade
                    python3 -m pip install pytest
                    python3 -m pytest
                '''
            }
        }
    }
}
