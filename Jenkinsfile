pipeline {
  agent any
  stages {
    sstage('Deploy to DEV') {
      steps {
         script {
            dockerHome = tool 'Docker'
            sh "${dockerHome}/bin/docker version"
           }
        }
    }
  }
}
