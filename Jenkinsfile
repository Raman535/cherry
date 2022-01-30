@Library('raman-demo') _
pipeline {
  agent any
  stages {
    stage('hello') {
       when {
        expression {
                  sample "$admin"
        }
      }
      steps {
        echo 'Please check the branch name'
        }
      }
    }

  }
}
