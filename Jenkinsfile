@Library('raman-demo') _
pipeline {
  agent any
  stages {
    stage('hello') {
      steps {
        echo 'hi raman'
        return = sample "$admin"
        if (!return) {
           error("Invalid branch name: ${admin}")
        }
      }
    }

  }
}
