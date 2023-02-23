pipeline {
  agent any
  stages {
    stage('Dev') {
      steps {
        echo 'I want to develope'
      }
    }

    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            echo 'I want to build'
          }
        }

        stage('test') {
          steps {
            echo 'i want to test'
          }
        }

        stage('deploy') {
          steps {
            echo 'i want to deploy'
          }
        }

      }
    }

  }
}