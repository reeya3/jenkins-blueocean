pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh '''pwd
date
cal'''
      }
    }

    stage('test') {
      parallel {
        stage('test') {
          steps {
            echo 'test1'
          }
        }

        stage('test2') {
          steps {
            echo 'test2'
          }
        }

      }
    }

    stage('deploy') {
      steps {
        sleep 10
      }
    }

  }
}