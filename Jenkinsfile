pipeline {
  agent any
  stages {
    stage('Checkout') {
      steps {
        echo 'Checkout stage'
        dir(path: 'env:WORKSPACE') {
          echo 'Inside workspace'
        }

        powershell 'Get-ChildItem'
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