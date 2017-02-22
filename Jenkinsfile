node {
  stage 'Checkout'
  checkout scm

  //def mvnHome = tool 'M3'
  env.PATH = "${tool 'apache-maven-3.3.9'}/bin:${env.PATH}"

  stage 'Build the JAR'
  
  //sh "${mvnHome}/bin/mvn -Dmaven.test.failure.ignore clean package"
  sh "mvn clean package"
  }
