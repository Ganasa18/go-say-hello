pipeline {
  agent any
  stages {
    stage('Prepare Environtement') {
      steps {
        echo 'Prepare Environtment'
        sh 'ls -la'
        sh 'printf develope openssl dgst -r -sha256 -hmac sregitops'
        script {
          docker ps
        }

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