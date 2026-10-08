pipeline {
    agent any
    triggers {
        pollSCM '* * * * *'
    }
    
    stages {
        stage('Build') {
            steps {
                echo "Building.."
                shh 'ls -ltr'
            }
        }
        stage('Test') {
            steps {
                echo "Testing.."
                sh 'echo "1111" > text'
            }
        }
        stage('Deliver') {
            steps {
                echo 'Deliver....'
                sh '''
                ls -ltr
                echo 'OK'
                '''
            }
        }
    }
}