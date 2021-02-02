pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                mvn compile
            }
        }
        stage('Test') {
            steps {
                mvn clean test
            }
        }
        stage('Deploy') {
            steps {
                mvn package
            }
        }
    }
}