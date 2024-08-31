pipeline {
  agent any
  stages {
    stage('plan') {
      steps {
        echo 'plan mode'
      }
    }

    stage('dev') {
      steps {
        echo 'development stage'
      }
    }

    stage('code') {
      steps {
        echo 'coding stage'
      }
    }

    stage('test') {
      parallel {
        stage('test') {
          steps {
            echo 'testing phase'
          }
        }

        stage('release') {
          steps {
            echo 'releasing stage'
          }
        }

        stage('deploy') {
          steps {
            echo 'deployment stage'
          }
        }

        stage('operate') {
          steps {
            echo 'operating stage'
          }
        }

      }
    }

  }
}