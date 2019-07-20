pipeline {
agent any 
  stages {
    stage ('Build') {
      steps {
        echo 'building now'
        sh './gradlew build --no-daemon'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
   }
}
