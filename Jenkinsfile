pipeline {
  agent any
  stages {
    stage('stage1') {
      steps {
        echo 'Thsi is $BUILD_NUMBER'
        sh 'echo "This is build number $BUILD_NUMBER"'
      }
    }

  }
  environment {
    DEMO = '1'
  }
}