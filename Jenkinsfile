pipeline {
  agent any

  stages {
    stage('Stage A') {
      parallel {
        stage('Stage B') {
          stage('Stage B1') {
          }
          stage('Stage B2') {
          }
          stage('Stage B3') {
          }
        }
        stage('Stage C') {
          stage('Stage C1') {
          }
          stage('Stage C2') {
          }
          stage('Stage C3') {
          }
        }
      }
    }
  }
}
