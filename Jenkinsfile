pipeline {
    agent any 
    stages {
        stage('Check docker-compose version') {
            steps {
                withEnv(['PATH+EXTRA=/usr/local/bin']) {
                    sh 'docker-compose --version'
                    sh 'cd Travelling_Managment/Travelling_Managment'
                    sh 'pwd'
                    sh 'ls -la'
                    //sh 'docker-compose build'
                    //sh 'docker-compose up'
                }
            }
        }
    }
}
