pipeline{
	agent any

	stages{
		stage('Compile Stage'){
			steps{
				maven(maven :'localmaven'){
					sh 'mvn clean compile'
				}
			}
		}
		stage('Testing Stage'){
			steps{
				maven(maven :'localmaven'){
					sh 'mvn test'
				}
			}
		}
		stage('Deploy Stage'){
			steps{
				maven(maven :'localmaven'){
					sh 'mvn deploy'
				}
			}
		}
	}
}
