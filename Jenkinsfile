pipeline {
  node (label 'slave11')
  stages {
    stage('print') {
      parallel {
        stage('print') {
          steps {
            echo 'hi'
          }
        }

        stage('print1') {
          steps {
            echo 'hello'
          }
        }

        stage('print3') {
          steps {
            echo 'how r u'
          }
        }

      }
    }

    stage('comming') {
      steps {
        sleep 30
      }
    }

    stage('end') {
      steps {
        echo 'end of pl'
      }
    }

  }
}
