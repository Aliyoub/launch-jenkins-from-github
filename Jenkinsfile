pipeline {
  stage('Initialize'){
        def dockerHome = tool 'MyDockerForPipeline'
        env.PATH = "${dockerHome}/bin:${env.PATH}"
  }
  stages {
    stage('Build') {
      steps {
        sh 'docker build -t abimimi-alpine .'
      }
    }
  }
}
