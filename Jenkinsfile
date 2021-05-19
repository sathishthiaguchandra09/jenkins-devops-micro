pipeline {
	agent { 
		docker { 
			image 'node:16.1'
			args '-u root:root'
		       } 
	      }
	stages {
		stage ('Build') {
			steps {
				sh 'node --version'
				echo "Build"
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
