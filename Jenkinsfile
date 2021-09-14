pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        nodejs('nodejs') {
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