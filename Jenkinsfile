pipeline {
  agent any
  stages {
    stage('Compile') {
      steps {
        echo 'compile'
      }
    }
    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo 'Test Unit code'
          }
        }
        stage('Test ui') {
          steps {
            echo 'ui test'
          }
        }
      }
    }
    stage('Productions') {
      steps {
        echo 'productions'
      }
    }
  }
}