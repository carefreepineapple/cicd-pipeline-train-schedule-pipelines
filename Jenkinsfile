pipeline {
  agent any
  stages {
    stage ('Build') {
      steps {
        echo 'Running  build automation'
        sh './gradlew build --no-daemon'
        archiveAritfacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
