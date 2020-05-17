pipeline {
  agent any
  stages {
    stage('print') {
      parallel {
        stage('print') {
          steps {
            echo 'hello'
          }
        }

        stage('clean') {
          steps {
            sleep 30
          }
        }

      }
    }

    stage('end') {
      steps {
        echo 'end of pl'
      }
    }

  }
}