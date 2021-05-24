node{
	stage('SCM Checkout'){

		git 'https://github.com/praveen-1989/devops1.git'
	}
	stage('Clean The Repo'){
		// Get maven home path 
		def mvnHome = tool name: 'maven-3', type: 'maven'
		bat "${mvnHome}/bin/mvn clean"
	}
	stage('Validate The Code'){
		// Get maven home path 
		def mvnHome = tool name: 'maven-3', type: 'maven'
		bat "${mvnHome}/bin/mvn validate"
	}
	stage('Compile the code'){
		// Get maven home path 
		def mvnHome = tool name: 'maven-3', type: 'maven'
		bat "${mvnHome}/bin/mvn compile"
	}
	stage('Test the code'){
		// Get maven home path 
		def mvnHome = tool name: 'maven-3', type: 'maven'
		bat "${mvnHome}/bin/mvn test"
	}
	stage('Package the code'){
		// Get maven home path 
		def mvnHome = tool name: 'maven-3', type: 'maven'
		bat "${mvnHome}/bin/mvn package"
	}
	stage('Install the Code'){
		// Get maven home path 
		def mvnHome = tool name: 'maven-3', type: 'maven'
		bat "${mvnHome}/bin/mvn install"
	}

}
