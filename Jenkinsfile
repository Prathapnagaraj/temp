pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo '"Hello"'
        bat(script: 'echo "hello"', returnStdout: true, returnStatus: true)
      }
    }

    stage('test') {
      steps {
        echo 'hello'
      }
    }

  }
  environment {
    MYVAR = '10'
  }
}