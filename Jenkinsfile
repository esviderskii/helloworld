pipeline {
    agent any 
    stages {
        stage('Stage 1') { 
            steps { 
                sh 'pwd' 
            }
        }
        stage('Stage 2'){
            steps {
                sh 'ls -lah' 
            }
        }
        stage('Test') {
            steps {
		echo(env.BRANCH_NAME)
                ifTest()
            }
        }
    }
}

def ifTest(){
        if ("${GIT_BRANCH}" == "origin/development") {
            echo('master')
        } else {
            echo("dev")
        }
}
