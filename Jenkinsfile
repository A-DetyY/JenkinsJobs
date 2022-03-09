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
        pysh 'update_project.py'
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