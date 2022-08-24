pipeline {
  agent any
  stages {
    stage('Checkout') {
      steps {
        echo 'Checkout stage'
        dir(path: 'env:WORKSPACE')
        bat(script: 'dir "%~dp0"', encoding: 'UTF-8', label: 'List Directory')
      }
    }

    stage('Build') {
      steps {
        echo 'Build Stage'
      }
    }

    stage('Test') {
      steps {
        echo 'Test Stage'
      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploy Stage'
      }
    }

  }
}