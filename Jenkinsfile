pipeline {
    agent any
    stages {
        
        stage('Build') {
            steps {
                echo 'Running build automation'
            }
        }   
          
        
        stage('Build Docker Image') {
            steps {
                script {
                    sh 'docker build . -t tech-blog'
                }
                
            }
        }   
      }
}
