pipeline {
    agent any 
    stages {
        stage('Build') { 
            steps { 
                sh 'pwd' 
            }
        }
        stage('Test'){
            steps {
                sh 'ls -lah' 
            }
        }
        stage('Deploy') {
            steps {
                sh 'uptime'
            }
        }
    }
}
