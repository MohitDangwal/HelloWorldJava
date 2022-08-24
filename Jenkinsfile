pipeline {
  agent any
  stages {
    stage('Checkout') {
      steps {
        echo 'Checkout stage'
        dir(path: 'env:WORKSPACE')
        git(url: 'git@github.com:MohitDangwal/HelloWorldJava.git', credentialsId: 'GithubHelloWorld')
        bat(script: 'dir', returnStatus: true, returnStdout: true)
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