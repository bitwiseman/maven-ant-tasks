pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'One Stage Build Pipeline'
      }
    }
  }
  environment {
    test2 = 'value2'
    test3 = '${test2}'
  }
}