pipeline{
  agent any
  stages{
    stage ('build') {
      steps {
        echo "Running Train Schedule Build"
        sh './gradlew build --no-deamon'
        archiveArtifacts artifact: 'dist/trainSchedule.zip'
      }
    }
  }
}
