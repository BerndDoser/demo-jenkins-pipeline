#!groovy

node('docker-host')
{
    stage('Build')
    {
        echo 'Build'
    }

    stage('Test')
    {
        echo 'Test'
        junit 'reports/*.xml'
    }

    stage('Deploy')
    {
        echo 'Deploy'
    }
}
