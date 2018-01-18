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
        steps {
          slackSend color: "good", message: "Woohoo.. New build ready for deployment. Approve? (<${env.BUILD_URL}|Open>)"
          input(message: 'Can I deploy?', ok: 'Go Ahead', id: '_ready')
        }
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