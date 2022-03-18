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

    stage('Notification') {
      steps {
        mail(subject: 'done', body: 'done', to: 'zhe.li4@pactera.com', from: 'marshal_li_b@163.com', charset: 'utf8')
      }
    }

  }
}