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
                // Wrap the maven command in sh or bat
                sh 'mvn clean package'
            }
        }
    }
}