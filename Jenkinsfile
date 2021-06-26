pipeline {

  agent none

  stages {
    stage("build") {
      agent { node {label 'master'}}
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