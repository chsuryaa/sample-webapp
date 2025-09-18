pipeline {
    agent any
    tools {
        maven 'M3'   // Use the Maven configured in Jenkins Global Tool Config
    }
    stages {
        stage('Build') {
            steps {
                sh 'mvn clean install'
            }
        }
        stage('Test') {
            steps {
                sh 'mvn test'
            }
        }
    }
}