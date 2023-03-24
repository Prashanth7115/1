pipeline {
  agent any
  stages {
    stage('1') {
      steps {
        sh '''pwd
free -h
'''
      }
    }

    stage('2') {
      parallel {
        stage('2') {
          steps {
            sh 'mkdir /media/1'
          }
        }

        stage('2.1') {
          steps {
            echo 'Creating a file in media'
          }
        }

      }
    }

    stage('3') {
      parallel {
        stage('3') {
          steps {
            sleep 4
          }
        }

        stage('') {
          steps {
            echo 'going to sleep for 4sec'
          }
        }

      }
    }

    stage('') {
      steps {
        sh 'll'
      }
    }

  }
}