@Library('raman-demo') _
pipeline {
  agent any
  stages {
    stage('hello') {
      steps {
        echo 'hi raman'
        result = sample "$admin"
        if (!result) {
           error("Invalid branch name: ${admin}")
        }
      }
    }

  }
}
