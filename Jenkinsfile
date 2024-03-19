
pipeline {
    agent any
    
    environment {
        APP_PORT = '9090'
    }
    
    stages {
        stage('Build') {
            steps {
                sh 'mvn clean package' // Use the maven package phase to build the project
            }
        }
        stage('Unit Test') {
            steps {
                sh 'mvn test' // Use the maven test phase to run unit tests
            }
        }
    }
}
