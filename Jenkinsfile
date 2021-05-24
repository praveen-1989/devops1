node{
	stage('SCM Checkout'){

		git 'https://github.com/praveen-1989/devops1.git'
	}
	stage('Copile-Package'){
		// Get maven home path 
		def mvnHome = tool name: 'maven-3', type: 'maven'
		sh "${mvnHome}/bin/mvn clean package"
	}
}
