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
        echo 'mvn clean install package'
      }
    }
  }
//  environment {
//    NAME = 'Hello World'
//  }
}
