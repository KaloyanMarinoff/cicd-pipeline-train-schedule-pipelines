pipeline{
  agent any
  
  stages{
    stage('Build'){
      steps{
        sh './gradlew build --no-daemon'
      }
    }
  }
  post{
    always{
      archiveArtifacts dist/trainSchedule.zip
    }
  }
}
