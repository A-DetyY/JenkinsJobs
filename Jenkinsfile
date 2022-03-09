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
        pybat(script: 'E:\\update_project.py', returnStatus: true, returnStdout: true)
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