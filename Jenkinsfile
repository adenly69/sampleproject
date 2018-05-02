pipeline {
  agent {
    docker {
      image 'maven:3-alpine'
    }

  }
  stages {
    stage('Run Unit Test') {
      steps {
        echo 'Running unit tests'
      }
    }
    stage('Create docker image') {
      steps {
        echo 'Create a new docker image'
      }
    }
    stage('Push to registry') {
      steps {
        echo 'Push image to registry'
      }
    }
    stage('Pull docker image') {
      steps {
        sh '/usr/bin/docker pull busybox'
      }
    }
  }
}