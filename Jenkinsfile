pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh '''pwd
./mvnw package'''
      }
    }

    stage('Deploy') {
      steps {
        sh 'java -jar target/*.jar'
      }
    }

  }
}