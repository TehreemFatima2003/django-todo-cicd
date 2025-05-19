pipeline {
  agent any
  stages {
    stage('Deploy') {
      steps {
        sh 'docker build -t todo .'
        sh 'docker run -d -p 8001:8000 todo'
      }
    }
  }
}
