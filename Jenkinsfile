pipeline {
  agent any
  stages {
    stage ('Build') {
    steps {
      echo 'Running from GIT forked Repo'
      sh './gradlew build --no-daemon'
      archiveArtifacts artifacts: 'dist/trainSchedule.zip'
    }
  }
  }
}
