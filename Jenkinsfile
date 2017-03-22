pipeline {
  agent any
  stages {
    stage('Test') {
      steps {
        node(label: 'osx_mbp') {
          sh 'echo "${test} ${test2}"'
        }
        
        echo '${test2} + ${test3}'
      }
    }
  }
  environment {
    test2 = 'value2'
    test3 = '${test2}'
  }
}