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
        sh 'docker bulid -t jenkins-laravel .'
      }
    }
  }
}

