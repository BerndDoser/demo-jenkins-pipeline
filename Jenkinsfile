#!groovy

pipeline {
  agent none 
  stages {
    stage('Build') {
      parallel (
        "Linux" : {
          steps {
            echo 'Build on Linux'
          }
        },
        "Mac" : {
          steps {
            echo 'Build on Mac'
          }
        },
        "Windows" : {
          steps {
            echo 'Build on Windows'
          }
        }
      )
    }
  }
}
