#!groovy

node('docker-host')
{
    stage('Build')
    {
        echo 'Build'
    }

    stage('Test')
    {
        def workspace = pwd()
        echo "Test workspace = ${workspace}"
        //junit 'reports/*.xml'
        step([$class: 'JUnitResultArchiver', testResults: 'reports/*.xml', healthScaleFactor: 1.0])
    }

    stage('Deploy')
    {
        echo 'Deploy'
    }
}
