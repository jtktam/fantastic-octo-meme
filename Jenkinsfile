pipeline {
  agent {
    docker {
      image 'maven:3.6.0-jdk-8-alpine'
    }

  }
  stages {
    stage('Build') {
      steps {
        sh '''echo PATH = ${PATH}
echo M2_HOME = ${M2_HOME}

mvn clean
'''
      }
    }
  }
}