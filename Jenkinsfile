pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh '''cd /var/lib/jenkins/workspace/spring-petclinic-1_main
./mvnw package'''
      }
    }

  }
}