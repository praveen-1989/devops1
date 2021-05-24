node{	
	
	def mvnHome = tool name: 'maven-3', type: 'maven'
	stage('SCM Checkout'){

		git 'https://github.com/praveen-1989/devops1.git'
	}
	stage('Clean The Repo'){

		bat "${mvnHome}/bin/mvn clean"
	}
	stage('Validate The Code'){

		bat "${mvnHome}/bin/mvn validate"
	}
	stage('Compile the code'){

		bat "${mvnHome}/bin/mvn compile"
	
	}
	stage('Package the code'){

		bat "${mvnHome}/bin/mvn package"

	}

}
