pipeline {
	agent any
	stages {
		stage('Checkout') {
			steps {
				checkout scm
			}
		}
		stage('Build') {
			steps {
				sh "mvn install"
			}
		}
		stage('Test') {
			steps {
				sh "mvn test"
			}
		}
		stage('Deploy') {
			steps {
				echo "War file deployed"
			}
		}
	}
}
