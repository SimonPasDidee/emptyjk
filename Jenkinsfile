pipeline {
  agent any
  stages {
    stage('Pre-before') {
      parallel {
        stage('Pre-before') {
          steps {
            echo 'oui'
          }
        }
        stage('error') {
          agent {
            node {
              label 'ansible'
            }

          }
          steps {
            sleep 2
            sleep 1
          }
        }
        stage('error') {
          steps {
            echo 'ddd'
          }
        }
        stage('error') {
          steps {
            echo 'ccc'
          }
        }
      }
    }
    stage('Before') {
      steps {
        echo 'non'
      }
    }
  }
}