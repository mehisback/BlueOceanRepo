pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'echo "build was ok"'
      }
    }

    stage('Deploy') {
      agent {
        node {
          label 'slave'
        }

      }
      steps {
        sh 'echo "Deployed successfully"'
        sh 'echo "nothing"'
      }
    }

  }
}