pipeline {
	agent { dockerfile true }
	
	stages {
		stage('Checkout') {
			git branch: 'master',
			credentialsId: 'gitaccess',															
			url: "${git_url}"																	
		}
		stage('Building') {
		    def customImage = docker.build("${userid}:${env.BUILD_ID}")
			echo 'Building the project'
			customImage.inside{
			sh('sample.sh')
			}
			customImage.push('latest')
		}
	}	
}