pipeline {
  agent any
  stages {
    stage('stage1') {
      steps {
        echo 'Thsi is $BUILD_NUMBER'
        sh 'echo "This is build number $BUILD_NUMBER"'
        stash(name: 'myfiles', includes: '*')
      }
    }

    stage('Approve for deployment') {
      steps {
        input(message: 'Approve Please', id: 'approveMessage', submitter: 'gnataraj', ok: 'Approved')
      }
    }

  }
  environment {
    DEMO = '1'
  }
}