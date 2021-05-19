pipeline {
	agent any
	stages {
		stage ('Build') {
			steps {
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
