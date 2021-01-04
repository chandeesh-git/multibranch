pipeline {
environment {
  BUILD_VERSION = "1.0"
}

    agent {
      label 'Docker'
    }


    stages {
	
	   stage('Build') {
	   when {
  environment name: 'BRANCH_NAME', value: 'dev'
}
	   
        steps {
		  
		  sh ' echo "Build ${BUILD_VERSION} stage success" '
		
          
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
  
 sh ' echo "Application Version ${BUILD_VERSION}" '
    // One or more steps need to be included within each condition's block.
  }
}
}
