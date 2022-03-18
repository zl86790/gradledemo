pipeline {
  agent any
  stages {
    stage('build') {
      parallel {
        stage('build1') {
          steps {
            sh 'echo "1"'
          }
        }

        stage('build2') {
          steps {
            sh 'echo "2"'
          }
        }

      }
    }

    stage('Clean') {
      steps {
        sh 'echo "clean"'
      }
    }

  }
}