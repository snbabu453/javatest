pipeline {
  agent any
  stages {
    stage('scm') {
      steps {
        git(url: 'https://github.com/jmstechhome/javatest.git', branch: 'master')
      }
    }

    stage('builds') {
      steps {
        sh '''javac HelloWorld.java
java HelloWorld'''
      }
    }

  }
}
