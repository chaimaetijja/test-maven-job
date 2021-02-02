pipeline {
    agent any
    tools {
    maven 'maven_3_5_4'
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