pipeline {
  agent any
  stages {
    stage ('build'){
      steps {
        echo 'running built automation'
        sh './gradlew build --no-daemon'
        archieveArtifacts artifacts:'ddist/trainSchedule.zip'
      }
    }
  }
}
