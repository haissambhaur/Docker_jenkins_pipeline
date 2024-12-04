pipeline {
    agent any 
    stages {
        stage('check version') {
            steps {
                sh 'docker --version'
                sh 'docker-compose --version'
            }
        }
    }
}
