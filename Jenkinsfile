pipeline {

  agent none

  stages {
    stage("build") {
      agent any
      steps {
        sh "docker -v"
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
