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
      }
    }

    stage('Packaging') {
      steps {
        echo 'Packaging'
        pysh 'packaging'
      }
    }

    stage('CommitIpa') {
      steps {
        echo 'CommitIpa'
        pysh 'commit_ipa'
      }
    }

  }
}