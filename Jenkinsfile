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
            mail(subject: 'from jenkins', body: 'test', to: 'yurturta@gmail.com', from: 'test@jenkins')
            echo 'prod'
          }
        }

      }
    }

  }
}