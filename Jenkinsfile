pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Build Start'
        sh 'mvn clean'
      }
    }
    stage('Test') {
      steps {
        echo 'Test Start'
      }
    }
  }
}