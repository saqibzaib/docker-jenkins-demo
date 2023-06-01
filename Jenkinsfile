pipeline {
  agent any
  stages {
    stage('image build') {
      steps {
        sh 'sudo docker build -t hello .'
      }
    }

    stage('container run') {
      steps {
        sh 'sudo docker run -d -p 3015:3000 hello'
      }
    }

  }
}
