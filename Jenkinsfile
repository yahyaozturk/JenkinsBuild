pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh '''node -v
npm -v'''
      }
    }
    stage('Static Code Anaysis') {
      steps {
        parallel(
          "Static Code Anaysis": {
            echo 'hello Word'
            
          },
          "Security Analysis": {
            echo 'hello Word'
            
          }
        )
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