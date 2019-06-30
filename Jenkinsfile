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
        stage('p1') {
          steps {
            echo 'Hi Dhamu'
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
        stage('p2') {
          steps {
            sh 'ls'
          }
        }
      }
    }
    stage('Deploy') {
      steps {
        echo 'Deploying....'
      }
    }
  }
  environment {
    NAME = 'rahul'
  }
}