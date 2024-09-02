pipeline {
  agent any
  stages {
    stage('Prepare Environtement') {
      steps {
        sh 'echo "Prepare environtment" ls'
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