pipeline {
  agent any
  stages {
    stage('Test') {
      steps {
        node(label: 'osx_mbp') {
          echo '${test}, ${test2}, ${test3}'
        }
        
      }
    }
  }
  environment {
    test = '${test3 + test2}'
    test2 = 'value2'
    test3 = '${test2}'
  }
}