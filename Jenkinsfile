pipeline{
 agent any
 stages {
 	stage('clone source') {
 	bat 'git clone'
 	}
 	
 	stage('Build project') {
 	bat 'mvn clean package'
 	}
 	
 	stage('Deploy') {
 	bat 'java -jar /target/*.jar'
 	}
 }
}