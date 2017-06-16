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
        echo 'Test'
        // Need new timestamp. Otherwise junit think tests were not running.
        sh 'touch reports/*.xml'
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
