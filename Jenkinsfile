pipeline {
  agent any
  stages {
    stage('Buzz Build') {
      steps {
        sh 'run_build.sh'
      }
    }

    stage('Buzz Test') {
      steps {
        sh './jenkins/test-all.sh'
      }
    }

  }
}