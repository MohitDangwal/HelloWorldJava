pipeline {
  agent any
  stages {
    stage('Checkout') {
      agent any
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
        bat 'javac HelloWorld.java'
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