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
                mvn clean package
            }
        }
    }
    
}
