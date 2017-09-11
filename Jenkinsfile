pipeline {
  agent any
  stage('build') {
    parallel (
      "win7-vs2012" : { stage("checkout") { }; stage("build") { }; stage("test") { } },
      "win10-vs2015" : { stage("checkout") { }; stage("build") { }; stage("test") { } },
      "linux-gcc5" : { stage("checkout") { }; stage("build") { }; stage("test") { } }
    )
  }
}
