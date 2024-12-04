pipeline {
    agent any 
    stages {
        stage('check version') {
            steps {
                sh 'docker-compose --version'
            }
        }
    }
}
