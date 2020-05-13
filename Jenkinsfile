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
        stage('Test') {
            steps {
                ifTest()
            }
        }
    }
}

def ifTest(){
        if ("${GIT_BRANCH}" == "origin/master") {
            echo('master')
        } else {
            echo("dev")
        }
}
