// Jenkinsfile (Declarative Pipeline)
pipeline {
  agent any
  stages {
    stage('Compile') {
      steps {
        mvn compile
      }
    }
    stage('Test') {
      steps {
        mvn clean test
      }
    }
    stage('Package') {
      steps {
        mvn package
      }
    }
  }
}