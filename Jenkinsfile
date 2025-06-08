pipeline{
	agent any
	tools{
		gradle 'Gradle'
		jdk 'JDK'
	}
	stages{
		stage('checkout'){
			steps{
				git branch:'master', url='https://github.com/AJITH-KUMAR-REDDY-RM/gradle44.git'
				}
			}
		stage('Build'){
			steps{
				sh 'gradle build'
			}
		}
		stage('Test')
		{
			steps{
				sh 'gradle test'
			}
		}
		stage('run')
		{
			steps{
				sh 'gradle run'
			}
		}
	}
	post{
		success{
			echo 'success'
			}
		failure{
			echo 'failure'
			}
	}
}
		
