pipeline {
  agent any

  stages {
    stage('Build') {
      steps {
        sh  'echo  "BUILD STAGE"'
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
        sh  'echo  "DEPLOY Develop"'
      }
      steps {
        sh  'echo  "DEPLOY STAGE"'
        sh  'ls -l'
      }
    }
  }
}