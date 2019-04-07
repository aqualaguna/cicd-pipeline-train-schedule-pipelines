pipeline {
  agent any
  stages {
    stage('Build') {
      echo 'Building Project...'
      sh './gradlew build --no-daemon'
      archiveArtifacts artifacts: 'dist/trainSchedule.zip'
    }
  }
}
