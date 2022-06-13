pipeline {
    agent any
    triggers {
        pollSCM('* * * * *')
    }
 
    stages {
        stage("Unit test") {
            steps {
                sh "/usr/bin/python3 test_calculator.py"
            }
        }
    }
}
