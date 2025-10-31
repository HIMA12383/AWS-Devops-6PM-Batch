pipeline {
  agent any
  stages {
    stage('plan') {
      steps {
        echo 'plan for dev'
      }
    }

    stage('code') {
      steps {
        echo 'plan the code'
      }
    }

    stage('build') {
      parallel {
        stage('build') {
          steps {
            echo 'build the code'
          }
        }

        stage('test') {
          steps {
            echo 'test the code'
          }
        }

        stage('deploy') {
          steps {
            echo 'deploy the code'
          }
        }

        stage('release') {
          steps {
            echo 'release the code'
          }
        }

        stage('operate') {
          steps {
            echo 'operate the code'
          }
        }

      }
    }

  }
}