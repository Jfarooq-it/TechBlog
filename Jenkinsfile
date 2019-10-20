pipeline {
    agent any
    stages {
        
        stage('Build') {
            steps {
                echo 'Running build automation'
            }
        }   
          
	    stage('Remove old Docker Container') {
      		steps {
			sh 'docker container rm tech-blog -f'
      }
    }
        
        stage('Build Docker Image') {
            steps {
                script {
                    sh 'docker build -t tech-blog .'
                }
                }
				}
          
	stage('Run Docker Container') {
      	    steps {
		    script {
			sh 'docker run --name tech-blog -d -p 8080:80 tech-blog'      
		}
                
            }
        } 
}
}
		
  
