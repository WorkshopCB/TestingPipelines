pipeline {
  agent any
  stages {
    stage('Stage1') {
      environment {
        MyVar = 'David'
      }
      steps {
        echo 'This is the first stage'
        sh '''echo ${MyVar}
'''
      }
    }
    stage('JDK') {
      steps {
        sh 'java -version'
      }
    }
  }
}