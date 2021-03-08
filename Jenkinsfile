pipeline {
  agent {
    dockerfile {
      filename 'Dockerfile'
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