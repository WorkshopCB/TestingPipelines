pipeline {
  agent any
  stages {
    stage('Stage1') {
      environment {
        MyVar = 'David'
      }
      steps {
        container('maven3'){
        echo 'This is the first stage'
        sh '''echo ${MyVar}
'''
          sh 'mvn --version'
        }
      }
    }
    stage('JDK') {
      steps {
        container('jdk8'){
        sh 'java -version'
        }
      }
    }
  }
}
