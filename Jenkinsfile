pipeline {
  agent any

  stages {
    stage('Build') {
      steps {
        sh  'echo  "BUILD STAGE"'
        sh  'apk update'
      }
    }
    stage('Test'){
      steps {
        sh  'echo  "TEST STAGE"'
        }
    }
    stage('Deploy'){
      when {
        branch 'develop'
      }
      steps {
        sh  'echo  "DEPLOY STAGE -----"'
        sh  'ls -l'
      }
    }
  }
}