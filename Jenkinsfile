pipeline {
  agent any
  stages {
    stage('scm') {
      steps {
        git(url: 'https://github.com/jmstechhome/javatest.git', branch: 'master', credentialsId: 'github_credentials')
      }
    }

    stage('build') {
      steps {
        sh '''javac HelloWorld.java
java HelloWorld'''
      }
    }

  }
}