pipeline{
	agent any
	tools {
   		maven
  	}
	stages {
		stage('checkout'){
			steps{
				checkout scm
			}
		}
		stage ('Build') {
        	//sh "echo 'shell scripts to build project...'"
			steps{
				sh "mvn package"
			}
			
        	}
	}
}
