pipeline{
 agent any
 	stages { 	
  	 stage('Clone source') {
 	steps {
 	checkout scm
 	}
 	}
 	stage('Build project') {
 	steps {
 	 bat 'mvn clean package'
 	}
 	}
 	
 	stage('Deploy') {
 	steps {
 	 bat 'java -jar ./target/bootJar.jar'
 	}
 	}
	stage('clean jenkins workspace') {
	steps {
	  cleanWs()
	}
	}
 }
}