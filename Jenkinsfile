pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh '''pwd
./mvnw package'''
      }
    }

    stage('Test') {
      steps {
        sh 'java -jar target/*.jar &>/dev/null &'
      }
    }

  }
}