pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Running ${env.BUILD_ID} on ${env.JENKINS_URL}'
        node(label: 'build dock image') {
          sh 'docker build -t build .'
        }

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