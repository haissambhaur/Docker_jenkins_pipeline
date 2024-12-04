pipeline {
    agent any 
    stages {
        stage('Check docker-compose version') {
            steps{
                sh 'pwd'
                sh 'ls -la'
                sh 'cd Travelling_Managment/'
            }
            steps {
                withEnv(['PATH+EXTRA=/usr/local/bin']) {
                    sh 'docker-compose --version'
                    //sh 'cd Travelling_Managment/'
                    //sh 'docker-compose build'
                    //sh 'docker-compose up'
                }
            }
        }
    }
}
