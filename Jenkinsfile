pipeline {
	agent any
	stages('Compile Stage'){
		steps{
			withMaven(maven: 'maven'){
				sh 'mvn clean compile'
			}
		}
	}
	stages('Testing Stage'){
		steps{
			withMaven(maven: 'maven'){
				sh 'mvn test'
			}
		}
	}
	stages('Testing Stage'){
		steps{
			withMaven(maven: 'maven'){
				sh 'mvn install'
			}
		}
	}
    
}
