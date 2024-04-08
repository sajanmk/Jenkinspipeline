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
            echo '"get the driver path $[ChromeDriverPath]"'
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
  environment {
    ChromeDriverPath = 'C:/Downloads/Driver/'
  }
}