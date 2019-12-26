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
 	 bat 'mvn springboot:run'
 	}
 	}
 }
}