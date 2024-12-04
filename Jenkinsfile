pipeline {
    agent any 
    environment {
        PATH = "/usr/local/bin:$PATH"  // Add the path to Docker Compose
    }
    stages {
        stage('check version') {
            steps {
                sh 'docker --version'
                sh 'docker-compose build'
                sh 'docker-compose up'
            }
        }
    }
}
