pipeline {
  agent any
  stages {
    stage('Pre-before') {
      parallel {
        stage('Pre-before') {
          steps {
            echo 'oui'
            echo 'ouiiii'
          }
        }
        stage('Before') {
          steps {
            echo 'non'
          }
        }
        stage('Oui') {
          steps {
            echo 'super'
          }
        }
      }
    }
    stage('ouais') {
      steps {
        echo 'fin'
      }
    }
  }
}