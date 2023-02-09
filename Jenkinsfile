@Library('folder-library') _

pipeline {
  agent {
    label 'linux'
  }
  
  stages {
    stage('Test') {
      script {
        steps {
          def t = get_time
          echo t
        }
      }
    }
  }
}
