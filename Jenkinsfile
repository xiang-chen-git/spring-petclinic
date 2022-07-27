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
        sh '''mvn clean verify sonar:sonar \\
  -Dsonar.projectKey=Petclinic \\
  -Dsonar.host.url=http://127.0.0.1:9000 \\
  -Dsonar.login=sqp_792227fbf974a1b253e811dae84429aa1fb654ef'''
      }
    }

  }
}