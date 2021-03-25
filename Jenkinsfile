pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Unit Test'
        echo 'Build'
      }
    }

    stage('Test') {
      steps {
        hygieiaBuildPublishStep(buildStatus: 'Success')
        echo 'Integration Testing'
      }
    }

    stage('Depoly') {
      steps {
        echo 'Deploying to AWS EC2'
      }
    }

  }
}