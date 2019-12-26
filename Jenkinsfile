pipeline{
 agent any
 stages { 	
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