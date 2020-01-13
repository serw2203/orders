pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh './mvnw clean package'
      }
    }
    stage('deploy') {
      steps {
        sh './mvnw fabric8:deploy'
      }
    }
  }
}