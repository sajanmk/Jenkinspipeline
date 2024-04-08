pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            echo 'building the docker image'
          }
        }

        stage('Test') {
          steps {
            echo 'testing the images'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'deploying the images'
      }
    }

  }
}