pipeline {
  agent any
  stages {
    stage('Test') {
      steps {
        node(label: 'osx_mbp') {
          sh 'echo "${test} ${test2}"'
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