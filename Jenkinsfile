pipeline {
  agent any
  tools {
        jdk 'jdk1.8'
        maven 'maven3.2.1'
    }
  stages {
    stage('Build') {
      steps {
        echo ' Cloning'
        //sh 'git clone https://github.com/varampati6/Hello_World.git'
      }
    }
    stage('Maven Build')
   {
     withEnv(["JAVA_HOME=${ tool 'jdk1.8' }", "PATH+M2_HOME=${tool 'maven3.2.1'}/bin:${env.JAVA_HOME}/bin", "MAVEN_OPTS=-Xms256m -Xmx256m -XX:NewSize=128m -XX:MaxNewSize=128m -XX:+UseG1GC -XX:+ExplicitGCInvokesConcurrent -XX:+ParallelRefProcEnabled -XX:+UseStringDeduplication -XX:+UnlockExperimentalVMOptions -XX:G1NewSizePercent=20 -XX:+UnlockDiagnosticVMOptions -XX:G1SummarizeRSetStatsPeriod=1"])
        {
         sh 'mvn -f ./pom.xml clean install org.jacoco:jacoco-maven-plugin:prepare-agent' 
        }
     sleep 10
   }
  }
//  environment {
//    NAME = 'Hello World'
//  }
}
