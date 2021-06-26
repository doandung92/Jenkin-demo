pipeline {

  agent none

  stages {
    stage("build") {
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
