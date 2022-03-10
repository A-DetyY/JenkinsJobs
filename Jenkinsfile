pipeline {
  agent any
  stages {
    stage('CheckRunningPlatform') {
      steps {
        echo 'CheckRunningPlatform'
        isUnix()
        echo 'Hello Hello'
      }
    }

    stage('UpdateProject') {
      steps {
        echo 'UpdateProject'
        echo 'LOL'
      }
    }

    stage('Packaging') {
      steps {
        echo 'Packaging'
      }
    }

    stage('CommitIpa') {
      steps {
        echo 'CommitIpa'
      }
    }

  }
}