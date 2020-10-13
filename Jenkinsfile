pipeline {
  agent {
    docker {
      image 'python:3.8-alpine'
    }

  }
  stages {
    stage('build') {
      steps {
        echo 'Building Applicaiton'
        sh 'sudo pip install -r requirements.txt'
      }
    }

    stage('test') {
      steps {
        echo 'Testing Applicaiton'
        sh 'pytest'
      }
    }

    stage('deploy') {
      steps {
        echo 'Deploying Applicaiton'
      }
    }

  }
}