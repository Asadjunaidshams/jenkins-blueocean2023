pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        echo 'build stage'
      }
    }

    stage('testing stage') {
      steps {
        echo 'testing stage'
      }
    }

    stage('operating stage') {
      parallel {
        stage('operating stage') {
          steps {
            echo 'operation of application'
          }
        }

        stage('compiling stage') {
          steps {
            echo 'compilation from maven'
          }
        }

        stage('exit stage') {
          steps {
            echo 'exit stage form application'
          }
        }

      }
    }

  }
}