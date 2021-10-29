pipeline {
  agent any
  stages {
    stage('image build') {
      steps {
        sh 'docker build -t hello .'
      }
    }

    stage('container run') {
      steps {
        sh 'docker run -d -p 3015:3000 hello'
      }
    }

  }
}
