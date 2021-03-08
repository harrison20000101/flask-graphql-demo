pipeline {
  agent {
    docker {
      image 'python'
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