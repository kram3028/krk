pipeline {
  agent any
  stages {
    stage('SCM Checkout') {
      steps {
        bat(script: 'git \\\'https://github.com/kram3028/my-app.git\\\'', returnStatus: true)
      }
    }

  }
}