pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        node(label: 'osx_mbp') {
          echo 'hello!'
        }
        
      }
    }
  }
  environment {
    test = '${test3}'
    test2 = 'value2'
    test3 = '${test2}'
  }
}