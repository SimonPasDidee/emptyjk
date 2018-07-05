pipeline {
  agent any
  stages {
    stage('Deployment 1st tier') {
      parallel {
        stage('Deployment 1st tier') {
          steps {
            sleep 1
          }
        }
        stage('Deployment 2nd tier') {
          steps {
            sh 'sleep 2'
            sleep 3
          }
        }
        stage('Deployment 3rd tier') {
          steps {
            sleep 2
            sleep 1
          }
        }
      }
    }
    stage('') {
      steps {
        sleep 3
      }
    }
  }
}