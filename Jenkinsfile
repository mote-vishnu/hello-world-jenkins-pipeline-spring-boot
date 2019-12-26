pipeline{
 agent any
 stages { 	
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
 }
}