pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        nodejs('node') {
          sh 'npm install'
        }

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