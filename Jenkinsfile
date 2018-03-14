pipeline{
	agent any
	stages {
		stage('checkout'){
		checkout scm
		}
		stage ('Build') {
        	//sh "echo 'shell scripts to build project...'"
		sh "mvn package"
			
        	}
	}
}
