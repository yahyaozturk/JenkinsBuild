pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'npm install'
        sh 'npm run build'
      }
    }
stage('SonarQube analysis') {
      steps {
        script {
          // requires SonarQube Scanner 2.8+
          scannerHome = tool 'SonarQube Default Scanner'
        }
        withSonarQubeEnv('Sonar') {
          sh "${scannerHome}/bin/sonar-scanner"
        }
      }
    }
    stage('Deploy to DEV') {
      steps {
        echo 'hello Word'
      }
    }
    stage('Smoke Test') {
      steps {
        parallel(
          "Smoke Test": {
            echo 'hello Word'
            
          },
          "Firefox": {
            echo 'hello Word'
            
          },
          "Chrome": {
            echo 'hello Word'
            
          },
          "IE": {
            echo 'hello Word'
            
          }
        )
      }
    }
    stage('Deploy to TEST') {
      steps {
        echo 'hello Word'
      }
    }
    stage('Regression Test') {
      steps {
        parallel(
          "Regression Test": {
            echo 'hello Word'
            
          },
          "Firefox": {
            echo 'hello Word'
            
          },
          "Chrome": {
            echo 'hello Word'
            
          },
          "IE": {
            echo 'hello Word'
            
          },
          "API": {
            echo 'hello Word'
            
          }
        )
      }
    }
    stage('Load Test') {
      steps {
        echo 'hello Word'
      }
    }
    stage('Deploy to Preprod') {
      steps {
        echo 'hello Word'
      }
    }
    stage('Merge to Master') {
      steps {
        echo 'hello Word'
      }
    }
  }
}
