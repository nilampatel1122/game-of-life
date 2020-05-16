pipeline {
  agent any
  stages {
    stage('Hello') {
      steps {
        echo 'Hi Hello'
      }
    }

    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            build(job: 'jenkinjob', quietPeriod: 30, wait: true)
          }
        }

        stage('Message') {
          steps {
            sh 'echo " This is first BO parallel pipeline"'
          }
        }

      }
    }

    stage('print') {
      steps {
        echo 'This is end of the project'
      }
    }

  }
}