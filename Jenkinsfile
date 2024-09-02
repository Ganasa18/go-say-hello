pipeline {
  agent any
  stages {
    stage('Prepare Environtement') {
      steps {
        echo 'Check out from version control'
      }
    }

    stage('Build') {
      steps {
        echo 'Checkout from version control'
        echo 'Building docker image'
      }
    }

    stage('Test') {
      steps {
        echo 'Testing'
      }
    }

  }
}