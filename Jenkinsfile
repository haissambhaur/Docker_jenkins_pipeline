pipeline {
    agent {
        docker {
            image 'ubuntu:20.04' 
            args '-u root'       
        }
    }
    stages {
        stage('Install Tools') {
            steps {
                sh '''
                apt-get update
                apt-get install -y docker.io curl
                curl -L https://github.com/docker/compose/releases/download/1.29.2/docker-compose-Linux-x86_64 -o /usr/local/bin/docker-compose
                chmod +x /usr/local/bin/docker-compose
                
                '''
            }
        }
        stage('check version') {
            steps {
                sh 'docker-compose --version'
            }
        }
    }
}
