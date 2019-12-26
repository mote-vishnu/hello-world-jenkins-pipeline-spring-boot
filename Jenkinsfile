pipeline{
 agent any
 	stages { 	
 	 stage('Clone source') {
 	steps {
 	bat 'git fetch'
 	}
 	}
 	stage('Build project') {
 	steps {
 	 bat 'mvn clean package'
 	}
 	}
 	
 	stage('Deploy') {
 	steps {
 	 bat 'java -jar /target/*.jar'
 	}
 	}
	stage('clean jenkins workspace') {
	steps {
	  cleanWs()
	}
	}
 }
}