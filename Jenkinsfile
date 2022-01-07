pipeline {
  agent any
  stages {
    stage('dev') {
      parallel {
        stage('dev') {
          steps {
            sh '''echo \'dev stage\'
'''
          }
        }

        stage('test') {
          steps {
            echo 'test stage'
          }
        }

        stage('production') {
          steps {
            echo 'prod'
            emailext(to: 'yurturta@gmail.com', subject: 'Test', body: 'Test')
          }
        }

      }
    }

  }
}