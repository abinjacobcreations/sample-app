pipeline {
  agent any
    
  tools {nodejs "node"}
    
  stages {
        
    stage('Git') {
      steps {
        git 'https://github.com/abinjacobcreations/sample-app.git'
      }
    }
     
    stage('Build') {
      steps {
        sh 'npm install'
         sh 'npm start'
      }
    }  
    
            
    stage('Test') {
      steps {
        sh 'node test'
      }
    }
  }
}