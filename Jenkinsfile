pipeline {
	agent any
	
	stages {
		stage('Checkout') {
			git branch: 'master',
			credentialsId: '',															# Should be incorporated from boilerplate repo.
			url: ''																		# Repo URL should be updated with the newly cloned repo details.
		}
		stage('Building') {
			echo 'Building the project'
			sh('sample.sh')
		}
	}	
}