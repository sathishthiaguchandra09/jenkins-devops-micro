pipeline {
	agent { docker { image 'maven:3.6.3'}}
		
	  stages {
		stage ('Build') {
			steps {
				#echo "Build"
				#echo "PATH - $PATH"
				#echo "BUILD_NUMBER - $env.BUILD_NUMBER"	
				#echo "BUILD_ID - $env.BUILD_ID"
				#echo "JOB_NAME - $env.JOB_NAME"
				#echo "BUILD_TAG - $env.BUILD_TAG"
				#echo "BUILD_URL - $env.BUILD_URL"
				sh 'mvn --version'
				echo 'build'
				#sh 'docker version'
				}
		}
		
		stage ('Test') {
			steps {
				echo "Test"
			}
		}
		
		stage ('Integration Test') {
			steps {
				echo "Integration test"
			}
		}
	}
	
	post {
		always {
			echo ' I m awesome'
		}
		
		success {
			echo 'its success'
		}
		
		failure {
			echo 'its failure'
		}
	}
}
