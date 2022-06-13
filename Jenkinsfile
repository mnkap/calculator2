pipeline {
    agent any
    triggers {
        pollSCM('* * * * *')
    }
 
    stages {
	stage('build') {
  	steps {
    		sh 'pip install -r requirements.txt'
  	}	
}
        stage("Unit test") {
            steps {
                sh "python3 test_calculator.py"
            }
        }
    }
}
