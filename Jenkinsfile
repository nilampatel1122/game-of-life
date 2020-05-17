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

        stage('sleep') {
          steps {
            sleep 30
          }
        }

      }
    }

    stage('print1') {
      steps {
        sh 'echo "finish"'
      }
    }

  }
}