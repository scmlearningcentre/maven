pipeline {
    agent any
    stages {
        stage('Example') {
           steps { bat "exit 1" }
        }
    }
    post { 
	failure {
	   mail body: 'Hi Adam', subject: 'The Pipeline failed', to: 'scmlearningcentre@gmail.com'
        }
    }
}

