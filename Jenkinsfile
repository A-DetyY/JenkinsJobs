pipeline {
  agent any
  stages {
    stage('CheckRunningPlatform') {
      steps {
        echo 'CheckRunningPlatform'
        isUnix()
      }
    }

    stage('UpdateProject') {
      steps {
        echo 'UpdateProject'
        echo 'LOL'
        sh 'python3 E:\\update_project.py'
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