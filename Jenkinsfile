pipeline {
    agent any
    triggers {
        pollSCM('* * * * *')
    }
 environment {
      PATH="/usr/bin/python3/bin:$PATH"
    }
    stages {
        stage("Unit test") {
            steps {
                sh "python3 test_calculator.py"
            }
        }
    }
}
