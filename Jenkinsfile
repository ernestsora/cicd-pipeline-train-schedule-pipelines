pipeline {
  agent any
  stages{
    stage('build') { 
      steps {
        echo 'Building project'
        sh ./gradlew build --no-daemon
        archiveArtifacts artifacts: "dist/trainSchedule.zip"
      }
    }
  }
}
