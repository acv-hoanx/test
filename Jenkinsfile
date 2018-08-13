pipeline {
  agent any
  branches('develop'){
    steps {
      sh  'echo  "This branch develop"'
    }
  }
  branches('feature/#1'){
    steps {
      sh  'echo  "This branch feature/%231"'
    }
  }
  branches('feature/%231'){
    steps {
      sh  'echo  "This branch feature/%231"'
    }
  }
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
      steps {
        sh  'echo  "DEPLOY STAGE"'
      }
    }
  }
}