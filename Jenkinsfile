#!groovy

node  {
	
	stage('Checkout') {
		 git branch: 'main', url: 'https://github.com/Nithishkumar0064/java-example.git'
	} 
	
	stage('Test'){
		sh 'echo thos is test stage'
	}
	
	stage('Build stage') {
		sh 'mvn clenan install'
	}
	stage('Deployment'){
		sh 'cp ./target/*.war /opt/tomcat/webapps/'
	} 
}
