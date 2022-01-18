pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        echo 'build complated'
      }
    }

    stage('test2') {
      parallel {
        stage('test2') {
          steps {
            echo 'running test2'
          }
        }

        stage('test1') {
          steps {
            echo 'running test1'
          }
        }

      }
    }

    stage('Depoly') {
      steps {
        input(message: 'are you sure to  deploy', ok: 'yes')
        echo 'Depoly complated '
      }
    }

    stage('notify new build') {
      steps {
        echo 'notify complated'
      }
    }

  }
}