pipeline {
  agent any
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
    stage('') {
      steps {
        junit(testResults: 'test-output', allowEmptyResults: true)
      }
    }
  }
  tools {
    nodejs 'Node'
  }
}