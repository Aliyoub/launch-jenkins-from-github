pipeline {
  agent any
  environment {
    DOCKERHUB_CREDENTIALS = credentials('aliyoubinate-dockerhub')
  }
  stages {
    stage('Build') {
      steps {
        sh 'docker build -t abimimi-alpine .'
      }
    }
  }
}
