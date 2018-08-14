pipeline {
  agent any

  stages {
    stage('Build') {
      steps {
        sh  'echo  "BUILD STAGE"'
        sh  'composer -v'
      }
    }
    stage('Test'){
      steps {
        sh  'echo  "TEST STAGE"'
        }
    }
    stage('Deploy - Develop'){
      when {
        branch 'develop'
      }
      steps {
        sh  'echo  "DEPLOY DEVELOP -----"'
        sh  'ls -l'
      }
    }
    stage('Deploy - Production'){
      when {
        branch 'master'
      }
      steps {
        sh  'echo  "DEPLOY PRODUCTION -----"'
      }
    }
  }
}