env.Maven3.5.4 = '/opt/maven'
pipeline {
	agent any

	stages {
	   stage ('Compile Stage') {
		steps {
		   
			sh "'${Maven3.5.4}/bin/mvn' clean compile"
		}
       	   }
	
	
	stage ('Testing Stage') {
	  steps {
		
		   sh "'${Maven3.5.4}/bin/mvn' clean test"
   		}
	    }
	

	stage ('Deploy Stage') {
	  steps {
		
		   sh "'${Maven3.5.4}/bin/mvn' clean deploy"
   		
	    }
	}
    }
}
