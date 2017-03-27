pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'One Stage Build Pipeline'
      }
    }
    stage('Test') {
      steps {
        parallel(
          "Platform 1": {
            echo 'Branch 1'
            
          },
          "Platform 2": {
            echo 'Branch 2'
            
          },
          "Platform 3": {
            echo 'Branch 3'
            
          }
        )
      }
    }
    stage('Deploy') {
      steps {
        echo 'Deploy Message'
      }
    }
  }
  environment {
    test2 = 'value2'
    test3 = '${test2}'
  }
}