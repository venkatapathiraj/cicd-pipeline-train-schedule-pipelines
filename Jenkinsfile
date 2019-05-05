pipeline {
  agent any 
  stages {
    stage ('build') {
      steps {
        echo "the build is in progress"
        sh './gradlew build --no-deamon'
          archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
