pipeline {
  agent {
    node {
      label 'docker'
    }

  }
  stages {
    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo '"testing"'
          }
        }

        stage('Parallel') {
          steps {
            echo 'parallel runing'
          }
        }

      }
    }

    stage('Build') {
      steps {
        echo 'building'
      }
    }

    stage('Clean Up') {
      steps {
        echo 'cleaning environment'
      }
    }

  }
}