node{
  stage('Checkout'){
    git 'https://github.com/varampati6/Hello_World.git'
  }
  stage('Build'){
   def mvnHOME = tool name: 'maven3.2.1', type: 'maven'
   sh '${mvnHOME}/bin/mvn clean install package'
    }
  }  

