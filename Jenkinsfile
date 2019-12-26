pipeline{

 agent any
 try {
 	stages { 	
 	 stage('Clone source') {
 	steps {
 	bat 'git clone https://github.com/mote-vishnu/hello-world-jenkins-pipeline-spring-boot.git'
 	}
 	}
 	stage('Build project') {
 	steps {
 	 bat 'mvn clean package'
 	}
 	}
 	
 	stage('Deploy') {
 	steps {
 	 bat 'java -jar /hello-world-jenkins-pipeline-spring-boot/target/*.jar'
 	}
 	}
 }
 }
 finally {
 bat 'rm hello-world-jenkins-pipeline-spring-boot'
 }
}