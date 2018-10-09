pipeline {
  agent any
  tools {
        jdk 'jdk1.8'
        maven 'maven3.2.1'
    }
  stages {
    stage('Build') {
      steps {
        sh 'git clone https://github.com/varampati6/Hello_World.git'
      }
    }
    stage('Test') {
      steps {
        sh '/opt/maven_home/bin/mvn clean install package'
      }
    }
  }
//  environment {
//    NAME = 'Hello World'
//  }
}
