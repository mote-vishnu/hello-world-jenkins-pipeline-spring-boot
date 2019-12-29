pipeline{
 agent any
 	stages { 
 	 stage('clean jenkins workspace') {
	 steps {
	  cleanWs()
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
	
 }
}