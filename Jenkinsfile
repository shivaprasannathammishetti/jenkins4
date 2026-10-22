pipeline {
    agent any
    tools {
        maven 'Maven1'
    }
    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }
        stage('Build and Package') {
            steps {
                // Change 'sh' to 'bat' for Windows environments
                bat 'mvn clean package'
            }
        }
    }
}