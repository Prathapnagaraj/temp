pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo '"Hello"'
        bat(script: 'echo "hello"', returnStdout: true, returnStatus: true)
        bat 'echo "hello world"'
        py 'print "hello"'
        catchError(buildResult: 'success', message: 'success') {
          timestamps() {
            echo 'hello'
          }

        }

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
