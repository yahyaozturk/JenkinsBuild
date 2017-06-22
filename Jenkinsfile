pipeline {
  agent any
      tools {
        nodejs 'Node'
    }
  stages {
    stage('Deploy to DEV') {
      steps {
        sh 'npm --version'
        sh 'node --version'
        script {
          dockerHome = tool 'Docker'
          sh "${dockerHome}/bin/docker version"
        }        
      }
    }
  }
}
