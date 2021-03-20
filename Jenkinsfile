pipeline {
  agent any
  stages {
    stage ('Build') {
      steps {
        echo 'Running build automation. New changes are added'
        sh './gradlew build --no-daemon'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
