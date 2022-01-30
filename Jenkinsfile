@Library('raman-demo') _
pipeline {
  agent any
  stages {
    stage('hello') {
       when {
        expression {
                  (false == sample "$admin")
        }
      }
      steps {
        echo 'Please check the branch name'
        error "This pipeline stops here!"
        }
      }
  }
}
