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

    stage('Test3-1') {
      steps {
        echo 'Test3  complated '
      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploy complated'
      }
    }

    stage('notify new build') {
      steps {
        echo 'notify completed'
      }
    }

  }
}