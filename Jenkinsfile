pipeline {

  agent none

  stages {
    stage("build") {
      agent { node {label 'master'}}
      steps {
        sh "docker-compose up -d"
      }
    }
  }

  post {
    success {
      echo "SUCCESSFUL"
    }
    failure {
      echo "FAILED"
    }
  }
}