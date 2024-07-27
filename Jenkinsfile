pipeline {
    agent any

    tools {
        // Define any tools required for the pipeline, e.g., Maven, JDK
        // maven 'M3'
        // jdk 'JDK8'
    }

    environment {
        // Define any environment variables if needed
        // SOME_VAR = 'some_value'
    }

    stages {
        stage('Declarative: Tool Install') {
            steps {
                // Example of installing a tool
                // tool name: 'Maven', type: 'Maven', home: tool 'M3'
            }
        }

        stage('Checkout') {
            steps {
                git url: 'https://github.com/jeazamor/remotedevops.git', branch: 'main'
            }
        }

        stage('Build') {
            steps {
                bat 'echo Building...'
                // Replace the following with your build command
                // bat 'start /B some_command'
            }
        }

        stage('Test') {
            steps {
                bat 'echo Testing...'
                // Replace the following with your test command
                // bat 'some_test_command'
            }
        }
    }

    post {
        always {
            echo 'Pipeline finished!'
        }
        success {
            echo 'Pipeline succeeded!'
        }
        failure {
            echo 'Pipeline failed!'
        }
    }
}
