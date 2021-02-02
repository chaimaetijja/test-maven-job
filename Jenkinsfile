pipeline {
    agent any
    tools {
    maven 'apache-maven-3.6.3'
  }

    stages {
        stage('Build') {
            steps {
                bat 'mvn compile'
            }
        }
        stage('Test') {
            steps {
                bat 'mvn clean test'
            }
        }
        stage('Deploy') {
            steps {
                bat 'mvn package'
            }
        }
    }
}