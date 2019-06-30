pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            echo 'Building..'
          }
        }
        stage('') {
          steps {
            echo 'Hello'
          }
        }
      }
    }
    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo 'Testing..'
          }
        }
        stage('') {
          steps {
            echo 'Hello Test'
          }
        }
      }
    }
    stage('Deploy') {
      parallel {
        stage('Deploy') {
          steps {
            echo 'Deploying....'
          }
        }
        stage('') {
          steps {
            echo 'Hi Deploy'
          }
        }
      }
    }
  }
  environment {
    NAME = 'rahul'
  }
}