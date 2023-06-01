pipeline {
  agent any
  stages {
    stage('image build') {
      steps {
        sh 'sudo docker build -t hello-2 .'
      }
    }

    stage('container run') {
      steps {
        sh 'sudo docker run -d -p 3020:3000 hello-2'
      }
    }

  }
}
