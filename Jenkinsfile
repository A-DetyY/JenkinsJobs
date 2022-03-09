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
        pybat 'E:\\update_project.py'
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