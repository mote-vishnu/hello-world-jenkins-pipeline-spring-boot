pipeline{
 agent any
 stages {
 	stage('clone source') {
 	steps {
 	 'git clone'
 	}
 	}
 	
 	stage('Build project') {
 	steps {
 	 'mvn clean package'
 	}
 	}
 	
 	stage('Deploy') {
 	steps {
 	 'java -jar /target/*.jar'
 	}
 	}
 }
}