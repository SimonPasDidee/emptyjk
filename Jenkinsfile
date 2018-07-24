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
        stage('') {
          steps {
            sleep 1
          }
        }
        stage('') {
          steps {
            echo 'ddd'
          }
        }
        stage('') {
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