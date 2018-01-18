pipeline {
  agent any
  stages {
    stage('Initiallize') {
      steps {
        echo 'Checkout'
        echo 'Done'
      }
    }
    stage('Build') {
      steps {
        echo 'Build'
        echo 'Done'
      }
    }
    stage('Test') {
      steps {
        echo 'Unit Test'
        echo 'Done'
      }
    }
    stage('Static Code Assessment') {
      steps {
        echo 'Static Scan'
        echo 'Done'
      }
    }
    stage('Security Scan') {
      steps {
        echo 'Security Scan'
        echo 'Done'
      }
    }
    stage('Publish Artifacts') {
      steps {
        echo 'Publish'
        echo 'Done'
      }
    }
    stage('Ask Approval') {
      steps {
        input 'Go ahead with deployment?'
      }
    }
    stage('Deploy') {
      steps {
        echo 'Approval'
        echo 'Done'
      }
    }
  }
}