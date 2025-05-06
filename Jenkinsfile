pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git url: 'https://github.com/yourname/your-repo.git', branch: 'master'
            }
        }
        stage('Install') {
            steps {
                bat 'pip install -r requirements.txt'
            }
        }
        stage('Test') {
            steps {
                bat 'pytest'
            }
        }
    }
}
