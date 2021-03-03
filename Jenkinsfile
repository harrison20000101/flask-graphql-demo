pipeline {
  agent {
    dockerfile {
      filename 'Dockerfile'
    }

  }
  stages {
    stage('Build') {
      steps {
        echo 'Building...'
        sh 'docker build'
      }
    }

    stage('Test') {
      steps {
        echo 'Testing...'
      }
    }

    stage('Depoly') {
      steps {
        echo 'Deploying...'
      }
    }

  }
}