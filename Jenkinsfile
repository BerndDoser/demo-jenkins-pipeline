pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        parallel(
          "Linux": {
            echo 'Build on Linux'
            
          },
          "Mac": {
            echo 'Build on Mac'
            
          },
          "Windows": {
            echo 'Build on Windows'
            
          }
        )
      }
    }
    stage('Test') {
      steps {
        parallel(
          "Test Linux": {
            echo 'Test on Linux'
            
          },
          "Test Mac": {
            echo 'Test on Mac'
            
          }
        )
      }
    }
    stage('Deploy') {
      steps {
        echo 'Deploy'
      }
    }
  }
}