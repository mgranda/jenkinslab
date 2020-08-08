pipeline {
  agent any
  stages {
    stage('Fluffy Build') {
      steps {
        echo 'Build'
      }
    }

    stage('Fluffy Test') {
      steps {
        echo 'Test'
        sh 'sleep 5'
        sh 'echo Success!'
      }
    }

    stage('Fluffy Deploy') {
      steps {
        echo 'Deploy'
        sh 'echo Another Placeholder.'
      }
    }

  }
}