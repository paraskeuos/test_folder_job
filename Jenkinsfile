pipeline {
  agent {
    label 'linux'
  }
  
  stages {
    stage('Test') {
      steps {
          library identifier: 'test-library@main', retriever: modernSCM([$class: 'GitSCMSource', credentialsId: 'GITHUB_KEY', remote: 'git@github.com:paraskeuos/devops-internship-task1.git', traits: [gitBranchDiscovery()]])
        script {
          def t = get_time()
          println t
        }
      }
    }
  }
  
  post {
    always {
      cleanWs()
    }
  }
}
