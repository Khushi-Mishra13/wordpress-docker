pipeline{
	agent any
		stages{
			stage('checkout'){
				steps{
					checkout scm
				}
			}
			stage('validate'){
				steps{
					sh 'docker compose config --quiet'
				}
			}
			stage('check docker'){
				steps{
					sh 'docker compose ps'
				}
			}
		}
}
