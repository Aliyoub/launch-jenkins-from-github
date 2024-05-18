pipeline {
  agent any
  stages {
    stage('Initialize'){
      def dockerHome = tool 'MyDockerForPipeline'
      env.PATH = "${dockerHome}/bin:${env.PATH}"
    }
    stage('Build') {
      steps {
        sh 'docker build -t abimimi-alpine .'
      }
    }
  }
}
