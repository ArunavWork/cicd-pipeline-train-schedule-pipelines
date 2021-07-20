pipeline{
  agent any
  stages{
    stage('Build'){
      steps{
        echo 'Running Build Automation'
        sh './gradlew clean build --no-daemon'
        archiveArtifacts artifacts: 'dist/trainschedule.zip'
      }
    }
  }
}
