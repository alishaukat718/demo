pipeline {
  environment {
    registry = "https://registry.hub.docker.com/repository/docker/alishaukat718/demo"
    registryCredential = 'alishaukat718'
  }
  agent any
  stages {
    stage('Building image') {
      steps{
        script {
          docker.build registry + ":$BUILD_NUMBER"
        }
      }
    }
  }
}
