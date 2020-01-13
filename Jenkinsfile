pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'mvn clean package'
      }
    }
    stage('deploy') {
      steps {
        sh 'mvn fabric8:deploy'
      }
    }
  }
}