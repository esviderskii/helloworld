pipeline {
    agent any 
    stages {
        stage('Build') { 
            steps {
		echo("${GIT_BRANCH}") 
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
