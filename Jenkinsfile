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
        sh 'docker build -t jenkins-laravel .'
      }
    }
  }
}

