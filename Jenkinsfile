pipeline{
  agent any
  stages {
    stage ('Build'){
      steps {
        echo 'Starting build'
        sh './gradlew build --no-daemon'
        archiveArtifact artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
  
}
