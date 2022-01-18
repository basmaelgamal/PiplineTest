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
        echo 'Depoly complated '
      }
    }

  }
}