pipeline{
 agent any
 stages {
 	stage('clone source') {
 	 'git clone'
 	}
 	
 	stage('Build project') {
 	 'mvn clean package'
 	}
 	
 	stage('Deploy') {
 	 'java -jar /target/*.jar'
 	}
 }
}