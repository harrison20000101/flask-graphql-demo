pipeline {
  agent {
    docker {
      args '-p 80:5000'
      image 'docpython:3.10.0a6-windowsservercore-ltsc2016'
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