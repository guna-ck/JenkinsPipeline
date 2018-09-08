pipeline {
	agent any

	stages {
	   stage ('Compile Stage') {
		steps {
		   
			sh "'${mvn}/bin/mvn' clean compile"
		
       	   }
	}
	
	stage ('Testing Stage') {
	  steps {
		
		    sh "'${mvn}/bin/mvn' clean test"
   		
	    }
	}

	stage ('Deploy Stage') {
	  steps {
		
		    sh "'${mvn}/bin/mvn' clean deploy"
   		
	    }
	}
    }
 }
