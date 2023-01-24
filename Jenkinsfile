pipeline {
  agent any
  environment {
        PATH = "$PATH:/opt/apache-maven-3.8.3/bin"
    }
    stages {

	stage ('Build')  {
	    steps {
            sh "mvn package"
	    sh " sudo docker build -t java-app . "

        }    
   }

  }
  }
