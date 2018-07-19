pipeline {
  agent {
    node {
      label 'docker'
    }
    
  }
  stages {
    stage('checkout') {
      parallel {
        stage('checkout') {
          steps {
            echo 'abc'
          }
        }
        stage('abc') {
          steps {
            echo 'var2'
          }
        }
      }
    }
    stage('ddd') {
      steps {
        sh 'echo abc'
      }
    }
  }
  environment {
    var1 = '1'
    var2 = '2'
  }
}