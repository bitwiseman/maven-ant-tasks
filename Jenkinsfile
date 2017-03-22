pipeline {
  agent any
  stages {
    stage('Test') {
      steps {
        node(label: 'osx_mbp') {
          echo '${test}, ${test2}'
        }
        
      }
    }
  }
  environment {
    test = 'value'
    test2 = 'value2'
    test3 = '${test2}'
  }
}