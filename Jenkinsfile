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
        echo "branch name $admin does not adhere to /feature\/[0-9]+\.[0-9]+\.[0-9]+/'.... hence exiting"
        error "This pipeline stops here!"
        }
      }
    stage('stage2') {
      steps {
       echo "Hello raman"
      }
    }
  }
}
