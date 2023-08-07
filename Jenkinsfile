pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        mail(subject: 'blueocean2023', body: 'msg from blueocean practice 2023, Hot girl eating momos', cc: 'shaistamamdapur7@gmail.com ', from: 'asad.junaid04@gmail.com', to: 'shaistamamdapur7@gmail.com ')
      }
    }

    stage('Development') {
      steps {
        echo 'This is development page'
      }
    }

    stage('Testing') {
      steps {
        timestamps() {
          currentUserItemRoles(showAllRoles: true)
        }

        echo 'Hello testing'
      }
    }

    stage('Operation') {
      parallel {
        stage('Operation') {
          steps {
            echo 'This is operation monitoring of application'
          }
        }

        stage('') {
          steps {
            sh 'echo $date'
          }
        }

      }
    }

  }
}