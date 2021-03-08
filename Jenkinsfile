pipeline {
  agent {
    docker {
      image 'python'
      args '-p 80:5000'
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