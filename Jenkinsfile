pipeline {
  agent any
  stages {
    stage('Buzz Build') {
      steps {
        sh 'ls -l'
        sh './run_build.sh'
      }
    }

    stage('Buzz Test') {
      steps {
        sh './run_tests.sh'
      }
    }

  }
}