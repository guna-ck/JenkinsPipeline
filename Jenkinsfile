pipeline {
	agent any

	stages {
	   stage ('Compile Stage') {
		steps {
		   withMaven(maven : 'Maven3.5.4') {
			sh 'mvn clean compile'
		}
       	   }
	}
	
	stage ('Testing Stage') {
	  steps {
		withMaven(maven: 'Maven3.5.4') {
		   sh 'mvn test'
   		}
	    }
	}

	stage ('Deploy Stage') {
	  steps {
		withMaven(maven: 'Maven3.5.4') {
		   sh 'mvn deploy'
   		}
	    }
	}
    }
}
