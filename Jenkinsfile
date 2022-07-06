pipeline{
  agent any
  
  stages{
    stage('Build'){
      steps{
        sh './gradlew build --no-daemon'
        archiveArtifacts: dist/trainSchedule.zip
      }
    }
  }
}
