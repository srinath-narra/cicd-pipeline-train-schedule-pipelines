pipeline{
  agent any
  stages{
    stage('Build'){
      steps{
        echo 'Running Build Automation'
        sh './gradleBuild --no-daemon'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
