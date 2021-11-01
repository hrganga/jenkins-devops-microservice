//SCRIPTED
// Declarative pipeline
pipeline {
		//agent any
		agent any
		stages{
			stage('Build'){
		steps{
		sh 'mvn --version'
        echo 'Build'
		}
		}
		stage('Test'){
		steps{
        echo 'Test'
		}
		}
		stage('Intergation Test'){
		steps{
        echo 'Integration Testing'
		}
		}
		}
		post{
			always{
				echo 'I run always'
			}
			success{
				echo 'I run only when success'
			}
			failure{
				echo 'I run only when failed'
			}
			changed{
				echo 'I run only when build status changed'
			}
		}
		
}
