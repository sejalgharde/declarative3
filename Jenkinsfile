pipeline {
	agent any 
	stages {
	    stage('Checkout') {
	        steps {
			checkout scm			       
		      }}
		stage('Build') {
	           steps {
			  sh '/home/sejal/Documents/devops-software/apache-maven-3.9.6/bin/mvn install'
	                 }}
		stage('Deployment'){
		   steps {
		sh 'cp target/declarative3.war /home/sejal/Documents/devops-software/apache-tomcat-9.0.85/webapps'
			}}	
}}
