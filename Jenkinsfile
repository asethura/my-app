pipeline{
	agent any
	tools {
   		maven 'Maven 3.3.9'
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
			BUILD_VERSION_GENERATED = VersionNumber(
			versionNumberString: '7.6.2.${BUILDS_ALL_TIME, X}',
        		projectStartDate:    '1970-01-01',
        		skipFailedBuilds:    true)
			currentBuild.displayName = BUILD_VERSION_GENERATED
			
        	}
	}
}
