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
        
      }
  }
    
    stage('Unit Testing') {
      steps {
        
        echo "Running Unit Tests"
        sh 'mvn test'
        sh mvn -v'
        
      }
    }
    
    stage('code Analysis') {
      steps {
        
        echo "Running Code Analysis"
        
      }
    }
    
    stage(Build Deploy Code') {
          when {
             branch 'develop'
          }
          steps {
            
            echo "Build Artifact"
            
            echo "Deploying code"
            
          }
       }
        
