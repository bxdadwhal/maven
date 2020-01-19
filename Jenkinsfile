pipeline {
    agent ec2-54-85-4-231.compute-1.amazonaws.com
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

