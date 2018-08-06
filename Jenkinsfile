pipeline {
	agent any
	
	stages {
		stage('Checkout') {
			steps {
				echo 'Checking out the project'
				checkout scm		
			}						
		}
		stage('Build') {
			steps {	
				echo 'Building the project'
				echo 'Thank you for building the project'
			}
		}
	}	
}
