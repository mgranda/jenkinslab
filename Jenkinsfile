pipeline {
  agent any
  stages {
    stage('Prepare Build') {
      steps {
        script {
          try {
            sh 'jar cvf target/demoapp.jar Foo.class'
          } catch(Exception e) {
            echo 'Error en generar jar ${env.BRANCH_NAME}'
          }
        }

      }
    }

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