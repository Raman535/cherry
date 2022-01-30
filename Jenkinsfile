@Library('raman-demo') _
pipeline {
  agent any
  stages {
    stage('stage1') {
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
    stage('stage2') {
      echo "Hello raman"
  }
}
