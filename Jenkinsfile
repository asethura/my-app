pipeline{
	agent any
	tools {
   		maven 'M2'
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
