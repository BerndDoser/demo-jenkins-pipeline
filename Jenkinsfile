#!groovy

pipeline {
  agent none 
  stages {
    stage('Build') {
      parallel (
        "Linux" : {
          echo 'Build on Linux'
        },
        "Mac" : {
          echo 'Build on Mac'
        },
        "Windows" : {
          echo 'Build on Windows'
        }
      )
    }
  }
}
