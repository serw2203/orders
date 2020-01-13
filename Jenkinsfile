pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'chmod 755 mvnw'
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