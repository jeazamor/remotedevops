pipeline {
    agent any
    stages {
        stage('Hello') {
            steps {
                echo "Hello from DEMO branch"
            }
        }
        stage('print demo.txt') {
            steps {
                bat 'type demo.txt'
            }
        }
    }
}

