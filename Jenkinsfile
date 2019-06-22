pipeline {
    agent any
    environment {
        DOCKER_IMAGE_NAME = "tomcat"
    }
    stages {
        stage('Build') {
            
			steps {
                input 'Deploy to Production?'
                milestone(1)
                kubernetesDeploy(
                    kubeconfigId: 'kubeconfig',
                    configs: 'tomcat.yml',
                    enableConfigSubstitution: true
		            )
                //implement Kubernetes deployment here
            }
			
			
			
			
			
        }
 
        
                    
        }
    }
