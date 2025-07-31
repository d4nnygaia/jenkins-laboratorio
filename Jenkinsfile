pipeline {
  agent any
  stages {
    stage('Vertificar Docker') {
      steps {
        sh 'docker info'
      }
    }
    stage('Docker build'){
      steps{
        sh 'docker rmi jenkins-laravel'
        sh 'docker build -t jenkins-laravel .'
        sh 'docker run -d jenkins-laravel'
      }
    }
  }
}

