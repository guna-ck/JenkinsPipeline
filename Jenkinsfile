pipeline {
	agent any

	stages {
	   stage ('Compile Stage') {
		steps {
		   
			sh "'${mvn_3.5.4}/bin/mvn' clean compile"
		
       	   }
	}
	
	stage ('Testing Stage') {
	  steps {
		
		    sh "'${mvn_3.5.4}/bin/mvn' clean test"
   		
	    }
	}

	stage ('Deploy Stage') {
	  steps {
		
		    sh "'${mvn_3.5.4}/bin/mvn' clean deploy"
   		
	    }
	}
    }
 }
