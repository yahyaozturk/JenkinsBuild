pipeline {
  agent any
  stages {
    stage('Deploy to DEV') {
      steps {
         script {
            dockerHome = tool 'Docker'
            sh "${dockerHome}/bin/docker version"
           }
        }
    }
  }
}
