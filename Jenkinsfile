agent any
	tools{
	jdk 'jdk1.8'
	}
stages{
  stage('Checkout'){
    git 'https://github.com/varampati6/Hello_World.git'
  stage('Build'){
   def MAVEN_HOME = tool name: 'maven3.2.1', type: 'maven'
   sh '${mvnHOME}/bin/mvn clean install package'
    }
  }  
}
