pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Code Check'
        sh 'sonar-scanner -Dsonar.projectKey=flask -Dsonar.sources=. -Dsonar.host.url=http://69.230.231.193:9000 -Dsonar.login=2c91611201f2b42549343ef4038df83acd165932'
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
