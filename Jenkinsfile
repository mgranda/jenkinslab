pipeline {
  agent any
  stages {
    stage('Buzz Build') {
      steps {
        sh 'ls -l'
        sh 'chmod +x ./run_build.sh'
        sh './run_build.sh'
      }
    }

    stage('Buzz Test') {
      steps {
        sh 'chmod +x ./run_tests.sh'
        sh './run_tests.sh'
      }
    }

  }
}