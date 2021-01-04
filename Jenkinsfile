pipeline {

    agent {
      label 'Docker'
    }


    stages {
	
	   stage('Build') {
	   
        steps {
		  
		  sh ' echo "Build stage success" '
		
          
		}
	   }
		
	   stage('Test') {
	   
        steps {
		  
		  sh ' echo "Test stage success" '
		
          
		}
	   }	
		
		stage('Deployment') {
	   
        steps {
		  
		  sh ' echo "Deployment stage success" '
		
          
		}

       }
       
    }   
	
	post {
  always {
  
 sh ' echo "Post build Actions" '
    // One or more steps need to be included within each condition's block.
  }
}
}
