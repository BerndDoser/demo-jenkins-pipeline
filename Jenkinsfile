#!groovy

pipeline
{
  agent any

  stages
  {
    stage('Build')
    {
      steps
      {
        echo 'Build'
      }
    }

    stage('Test')
    {
      steps
      {
        echo "Test"
        junit 'reports/*.xml'
      }
    }

    stage('Deploy')
    {
      steps
      {
        echo 'Deploy'
      }
    }
  }
}
