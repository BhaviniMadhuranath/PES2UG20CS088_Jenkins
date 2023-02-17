pipeline {
	agent any
	stages {
		stage('Build')	{
			steps {
				sh 'g++ new_hello.cpp -o exte'
				echo 'Build Stage Successful'
			}
		}
		stage('Test')	{
			steps {
				sh './execute'
				echo 'Test Stage Successful'
			}
		}
		stage('Deploy')	{
			steps {
				echo 'Deploy Stage Successful'
			}
		}
	}
	post {
		failure {
			echo 'Pipeline failed'
		}
	}
}
