pipeline {
  agent any
  stages {
    stage('scsm') {
      steps {
        git(url: 'https://github.com/jmstechhome/javatest.git', branch: 'master')
      }
    }

    stage('builsds') {
      steps {
        sh '''javac HelloWorld.java
java HelloWorld'''
      }
    }

  }
}
