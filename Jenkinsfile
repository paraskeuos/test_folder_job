@Library('folder-library') _

pipeline {
  agent {
    label 'linux'
  }
  
  stages {
    stage('Test') {
      steps {
        script {
          def t = get_time
          echo t
        }
      }
    }
  }
}
