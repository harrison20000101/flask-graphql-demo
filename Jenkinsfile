pipeline {
  agent {
    docker {
      args '-p 80:5000'
      image 'python:3.10.0a6-alpine3.13'
    }

  }
  stages {
    stage('Build') {
      steps {
        sh '''RUN pip install -r requirements.txt
'''
      }
    }

  }
  environment {
    CI = 'True'
  }
}