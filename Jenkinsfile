pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'git clone https://github.com/varampati6/Hello_World.git'
      }
    }
    stage('Test') {
      steps {
        echo 'Tesing'
      }
    }
  }
  environment {
    NAME = 'Hello World'
  }
}
