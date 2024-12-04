pipeline {
    agent any 
    stages {
        stage('check version') {
            steps {
                sh 'docker --version'
            }
            
            steps {
                sh 'docker-compose build'
            }
            
            steps {
                sh 'docker-compose up'
            }
        }
    }
}
