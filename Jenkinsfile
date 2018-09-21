pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        bat(script: 'echo "This is build', returnStatus: true)
      }
    }
    stage('Code_checkOut') {
      steps {
        git(url: 'infygit', branch: 'master', credentialsId: 'test', poll: true)
      }
    }
  }
}