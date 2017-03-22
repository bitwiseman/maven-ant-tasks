pipeline {
  agent any
  stages {
    stage('') {
      steps {
        echo '${test}, ${test2}, ${test3}'
      }
    }
  }
  environment {
    test = '${test3 + test2}'
    test2 = 'value2'
    test3 = '${test2}'
  }
}