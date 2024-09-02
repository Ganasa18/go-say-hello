pipeline {
  agent any
  stages {
    stage('Prepare Environtement') {
      steps {
        echo 'Prepare Environtment'
        sh 'ls -la'
        sh 'printf develope openssl dgst -r -sha256 -hmac sregitops'
        sh ''' def dockerfileExists = sh(script: \'test -f Dockerfile && echo "exists" || echo "not exists"\', returnStdout: true).trim()
                    if (dockerfileExists == \'exists\') {
                        echo \'Dockerfile exists.\'
                    } else {
                        error \'Dockerfile not found.\'
                    }'''
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