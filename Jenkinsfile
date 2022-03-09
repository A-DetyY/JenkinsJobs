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
        pysh '/var/jenkins_home/pyfiles/update_project.py'
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