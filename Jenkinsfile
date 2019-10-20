pipeline {
    agent any
    stages {
        
        stage('Build') {
            steps {
                echo 'Running build automation'
            }
        }   
        
        stage('Lint HTML') {
        steps {
          sh 'tidy -q -e *.html'
          }
        }
		  
        
        stage('Test') {
            steps {
                echo 'Testing second stage!'
            }
        }   
      }
}
