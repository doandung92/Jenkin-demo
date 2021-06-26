pipeline {

  agent none

  stages {
    stage("build") {
      agent { node {label 'master'}}
      steps {
        sh "echo 'Hello'"
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
