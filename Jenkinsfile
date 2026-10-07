pipeline {
    agent any
    triggers {
        pollSCM '*/2 * * * *'
    }
    
    stages {
        stage('Build') {
            steps {
                echo "Building.."
                sh 'ls -ltr'
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