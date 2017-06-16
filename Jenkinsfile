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
    def workspace = pwd()
    echo "Test workspace = ${workspace}"
    sh 'ls -al'
    //junit 'reports/*.xml'
    step([$class: 'JUnitResultArchiver', testResults: 'reports/*.xml', healthScaleFactor: 1.0])
  }

  stage('Deploy')
  {
    echo 'Deploy'
  }
}
