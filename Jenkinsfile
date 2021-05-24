node{
	stage('SCM Checkout'){

		git 'https://github.com/praveen-1989/devops1.git'
	}
	stage('Copile-Package'){
		// Get maven home path 
		def mvnHome = tool name: 'maven-3', type: 'maven'
		bat "${mvnHome}/bin/mvn clean"
	}
	stage('Copile-Package'){
		// Get maven home path 
		def mvnHome = tool name: 'maven-3', type: 'maven'
		bat "${mvnHome}/bin/mvn validate"
	}
	stage('Copile-Package'){
		// Get maven home path 
		def mvnHome = tool name: 'maven-3', type: 'maven'
		bat "${mvnHome}/bin/mvn compile"
	}
	stage('Copile-Package'){
		// Get maven home path 
		def mvnHome = tool name: 'maven-3', type: 'maven'
		bat "${mvnHome}/bin/mvn test"
	}
	stage('Copile-Package'){
		// Get maven home path 
		def mvnHome = tool name: 'maven-3', type: 'maven'
		bat "${mvnHome}/bin/mvn package"
	}
	stage('Copile-Package'){
		// Get maven home path 
		def mvnHome = tool name: 'maven-3', type: 'maven'
		bat "${mvnHome}/bin/mvn install"
	}

}
