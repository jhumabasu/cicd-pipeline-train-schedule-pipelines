pipeline{
  agent any
  stages{
    stage ('Build') {
      steps {
        echo 'Running Train Schedule Build'
        sh './gradlew build --no-daemon'
        archiveArtifacts artifact: 'dist/trainSchedule.zip'
      }
    }
  }
}
