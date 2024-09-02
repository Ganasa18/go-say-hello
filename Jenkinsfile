pipeline {
  agent any
  stages {
    stage('Prepare Environtement') {
      steps {
        echo 'Prepare Environtment'
        sh ''' def commitMessage = sh(script: \'git log -1 --pretty=format:"%H - %an, %ar : %s"\', returnStdout: true).trim()
                    echo "Latest commit: go-say-hello${commitMessage}"'''
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