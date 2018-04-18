pipeline {
  agent any
  stages {
    stage('checkout project') {
      steps {
        sh '''mvn test
'''
      }
    }
    stage('test') {
      steps {
        junit 'target/surefire-reports/*.xml'
      }
    }
  }
}