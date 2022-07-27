pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh '''cd spring-petclinic
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