pipeline {
  agent any
  stages {
    stage('SCM Checkout') {
      steps {
        bat(script: 'git \\\'https://github.com/kram3028/my-app.git\\\'', returnStatus: true)
      }
    }

    stage('Build') {
      steps {
        bat 'mvn clean package'
        build(job: 'war', quietPeriod: 20, wait: true)
      }
    }

  }
}