pipeline {
    agent any
    tools {
    maven 'apache-maven-3.6.3'
  }

    stages {
        stage('Build') {
            steps {
                sh 'mvn compile'
            }
        }
        stage('Test') {
            steps {
                sh 'mvn clean test'
            }
        }
        stage('Deploy') {
            steps {
                sh 'mvn package'
            }
        }
    }
}