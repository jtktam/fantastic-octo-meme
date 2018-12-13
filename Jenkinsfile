pipeline {
  agent {
    docker {
      image 'maven:3.6.0-jdk-8-alpine'
      args '-v "$HOME/.m2":/root/.m2'
    }

  }
  stages {
    stage('Build') {
      steps {
        sh '''echo PATH = ${PATH}
echo M2_HOME = ${M2_HOME}

mvn clean
mvn compile'''
      }
    }
  }
}