pipeline{
  agent any
  
  stages{
    stage('Build'){
      steps{
        ./gradlew build --no-daemon
        archiveArtifacts dist/trainSchedule.zip
      }
    }
  }
}
