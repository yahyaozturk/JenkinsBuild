pipeline {
  agent any
  stages {
    stage('Deploy to DEV') {
      steps {
        tool 'Node'
        sh '''node -v
npm -v'''
        script {
          dockerHome = tool 'Docker'
          sh "${dockerHome}/bin/docker version"
        }
        
      }
    }
  }
}