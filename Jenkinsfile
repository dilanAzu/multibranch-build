pipeline {
  
  agent any
      tools { 
           maven 'maven'
      }
    
  stages {
    
    stage('cleanup workspace') {
    steps {
        cleanws()
      
        echo "clean up workspace foe projects"
      
    }
 }
    
  stage('code checkout') {
      steps {
        
