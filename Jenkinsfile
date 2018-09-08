pipeline {
	agent any

	stages {
	   stage ('Compile Stage') {
		steps {
		   
			sh "'${MVN_HOME}/bin/mvn' clean compile"
		
       	   }
	}
	
	stage ('Testing Stage') {
	  steps {
		
		    sh "'${MVN_HOME}/bin/mvn' clean test"
   		
	    }
	}

	stage ('Deploy Stage') {
	  steps {
		
		    sh "'${MVN_HOME}/bin/mvn' clean deploy"
   		
	    }
	}
    }
 }
