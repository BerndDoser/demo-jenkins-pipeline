#!groovy

node('docker-host')
{
  stage('Checkout')
  {
    echo 'Checkout'
    git url: "https://github.com/BerndDoser/demo-jenkins-pipeline.git", branch: 'groovy-simple'
  }

  stage('Build')
  {
    echo 'Build'
  }

  stage('Test')
  {
    echo 'Test'
    // Need new timestamp. Otherwise junit think tests were not running.
    sh 'touch reports/*.xml'
    junit 'reports/*.xml'
  }

  stage('Deploy')
  {
    echo 'Deploy'
  }
}
