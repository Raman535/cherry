@Library('raman-demo') _
pipeline {
  agent any
  stages {
    stage('hello') {
      output = sample "$admin"
      echo "$output"
       when {
        expression {
                  sample "$admin"
        }
      }
      steps {
        echo 'Please check the branch name'
        error "This pipeline stops here!"
        }
      }
  }
}
